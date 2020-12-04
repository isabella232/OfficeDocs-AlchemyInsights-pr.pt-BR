---
title: Solucionar problema de PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571788"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="e01f6-102">Solucionar problema de PRT</span><span class="sxs-lookup"><span data-stu-id="e01f6-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="e01f6-103">Para qualquer dispositivo concluir a autenticação, ele deve estar totalmente registrado e em bom estado e ser capaz de adquirir um token de atualização principal (PRT).</span><span class="sxs-lookup"><span data-stu-id="e01f6-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="e01f6-104">O processo de registro de ingresso do Azure AD híbrido exige que os dispositivos estejam em uma rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="e01f6-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="e01f6-105">Ele também funciona pela VPN, mas há algumas advertências para isso.</span><span class="sxs-lookup"><span data-stu-id="e01f6-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="e01f6-106">Ouvimos clientes que precisam de assistência com a solução de problemas do processo de registro de ingresso do Azure AD híbrido em circunstâncias de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="e01f6-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="e01f6-107">Aqui está uma divisão do que está acontecendo, nos bastidores, durante o processo de registro.</span><span class="sxs-lookup"><span data-stu-id="e01f6-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="e01f6-108">**Ambiente de autenticação em nuvem (usando a sincronização de hash de senha ou autenticação de passagem do Azure AD)**</span><span class="sxs-lookup"><span data-stu-id="e01f6-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="e01f6-109">Esse fluxo de registro também é conhecido como "junção de sincronização".</span><span class="sxs-lookup"><span data-stu-id="e01f6-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="e01f6-110">O Windows 10 descobre um registro SCP quando o usuário faz logon no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e01f6-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="e01f6-111">O dispositivo primeiro tenta recuperar informações do locatário do SCP do lado do cliente no registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="e01f6-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="e01f6-112">Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="e01f6-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="e01f6-113">Se ele falhar, o dispositivo se comunica com o Active Directory (AD) local para obter informações de locatário do ponto de conexão de serviço (SCP).</span><span class="sxs-lookup"><span data-stu-id="e01f6-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="e01f6-114">Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="e01f6-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="e01f6-115">É recomendável habilitar o SCP no AD e usar somente o SCP do lado do cliente para validação inicial.</span><span class="sxs-lookup"><span data-stu-id="e01f6-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="e01f6-116">O Windows 10 tenta se comunicar com o Azure AD no contexto do sistema para se autenticar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e01f6-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="e01f6-117">Você pode verificar se o dispositivo pode acessar recursos da Microsoft na conta do sistema usando o script de conectividade de registro do dispositivo de teste.</span><span class="sxs-lookup"><span data-stu-id="e01f6-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="e01f6-118">O Windows 10 gera um certificado autoassinado e o armazena no objeto computador no AD local.</span><span class="sxs-lookup"><span data-stu-id="e01f6-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="e01f6-119">Isso exige uma linha de visão para o controlador de domínio.</span><span class="sxs-lookup"><span data-stu-id="e01f6-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="e01f6-120">Um objeto Device que tem um certificado é sincronizado com o Azure AD por meio do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e01f6-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="e01f6-121">O ciclo de sincronização é a cada 30 minutos por padrão, mas depende da configuração do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e01f6-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="e01f6-122">Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="e01f6-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="e01f6-123">Neste estágio, você deve ser capaz de ver o dispositivo de assunto no estado "pendente", em folha de dispositivo do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e01f6-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="e01f6-124">No próximo login do usuário no Windows 10, o registro será concluído.</span><span class="sxs-lookup"><span data-stu-id="e01f6-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="e01f6-125">Se você estiver na VPN e um processo de logon de logoff encerrar a conectividade do domínio, você pode disparar o registro manualmente:</span><span class="sxs-lookup"><span data-stu-id="e01f6-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="e01f6-126">Emita um dsregcmd/Join localmente no prompt de administrador ou remotamente via PSExec para seu computador.</span><span class="sxs-lookup"><span data-stu-id="e01f6-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="e01f6-127">Por exemplo, PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="e01f6-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="e01f6-128">Para obter mais detalhes sobre problemas de União híbrida, consulte [Troubleshoot Devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="e01f6-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
