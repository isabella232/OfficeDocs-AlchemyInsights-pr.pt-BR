---
title: Dispositivo em estado pendente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652110"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="16d9c-102">Dispositivo em estado pendente</span><span class="sxs-lookup"><span data-stu-id="16d9c-102">Device in pending state</span></span>

<span data-ttu-id="16d9c-103">**Pré-requisitos**</span><span class="sxs-lookup"><span data-stu-id="16d9c-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="16d9c-104">Se estiver configurando registros de dispositivo pela primeira vez, verifique se você analisou [a introdução ao gerenciamento de dispositivos no Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , que orientará você sobre como obter dispositivos sob o controle do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="16d9c-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="16d9c-105">Se você estiver registrando dispositivos no Azure AD diretamente e registrá-los no Intune, será necessário garantir que você tenha configurado o [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e ter o [Licenciamento](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) em vigor primeiro.</span><span class="sxs-lookup"><span data-stu-id="16d9c-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="16d9c-106">Certifique-se de que você está autorizado a executar operações no Azure AD e no AD local.</span><span class="sxs-lookup"><span data-stu-id="16d9c-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="16d9c-107">Somente um administrador global no Azure AD pode gerenciar configurações de registros de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="16d9c-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="16d9c-108">Além disso, se você estiver configurando registros automáticos no seu Active Directory local, será necessário ser um administrador do Active Directory e do AD FS (se aplicável).</span><span class="sxs-lookup"><span data-stu-id="16d9c-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="16d9c-109">O processo de registro de ingresso do Azure AD híbrido exige que os dispositivos estejam na rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="16d9c-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="16d9c-110">Ele também funciona pela VPN, mas há algumas advertências para isso.</span><span class="sxs-lookup"><span data-stu-id="16d9c-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="16d9c-111">Ouvimos clientes que precisam de assistência com a solução de problemas do processo de registro de ingresso do Azure AD híbrido em circunstâncias de trabalho remotas.</span><span class="sxs-lookup"><span data-stu-id="16d9c-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="16d9c-112">**Ambiente de autenticação em nuvem (usando a sincronização de hash de senha ou autenticação de passagem do Azure AD)**</span><span class="sxs-lookup"><span data-stu-id="16d9c-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="16d9c-113">Esse fluxo de registro também é conhecido como "junção de sincronização".</span><span class="sxs-lookup"><span data-stu-id="16d9c-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="16d9c-114">Veja a seguir uma análise do que acontece durante o processo de registro:</span><span class="sxs-lookup"><span data-stu-id="16d9c-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="16d9c-115">O Windows 10 descobre o registro do ponto de conexão de serviço (SCP) quando o usuário faz logon no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16d9c-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="16d9c-116">O dispositivo primeiro tenta recuperar informações do locatário do SCP do lado do cliente no registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="16d9c-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="16d9c-117">Para obter mais informações, consulte [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="16d9c-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="16d9c-118">Se ele falhar, o dispositivo se comunica com o Active Directory local para obter informações de locatário do SCP.</span><span class="sxs-lookup"><span data-stu-id="16d9c-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="16d9c-119">Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="16d9c-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="16d9c-120">É recomendável habilitar o SCP no Active Directory e usar somente o SCP do lado do cliente para validação inicial.</span><span class="sxs-lookup"><span data-stu-id="16d9c-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="16d9c-121">O Windows 10 tenta se comunicar com o Azure AD no contexto do sistema para se autenticar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="16d9c-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="16d9c-122">Você pode verificar se o dispositivo pode acessar recursos da Microsoft na conta do sistema usando o [script de conectividade de registro do dispositivo de teste](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="16d9c-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="16d9c-123">O Windows 10 gera um certificado autoassinado e o armazena no objeto computador no Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="16d9c-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="16d9c-124">Isso exige uma linha de visão para o controlador de domínio.</span><span class="sxs-lookup"><span data-stu-id="16d9c-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="16d9c-125">O objeto Device que tem o certificado é sincronizado com o Azure AD por meio do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="16d9c-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="16d9c-126">O ciclo de sincronização é a cada 30 minutos por padrão, mas depende da configuração do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="16d9c-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="16d9c-127">Para obter mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="16d9c-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="16d9c-128">Neste estágio, você deve ser capaz de ver o dispositivo de assunto no estado "**pendente**", em folha de dispositivo do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="16d9c-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="16d9c-129">No próximo login do usuário no Windows 10, o registro será concluído.</span><span class="sxs-lookup"><span data-stu-id="16d9c-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="16d9c-130">Se você estiver na VPN e o logoff/logon encerrar a conectividade do domínio, você poderá disparar o registro manualmente.</span><span class="sxs-lookup"><span data-stu-id="16d9c-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="16d9c-131">Para isso:</span><span class="sxs-lookup"><span data-stu-id="16d9c-131">To do that:</span></span>
    >
    > <span data-ttu-id="16d9c-132">Emita um `dsregcmd /join` aviso local no prompt de administrador ou remotamente via PsExec para seu computador.</span><span class="sxs-lookup"><span data-stu-id="16d9c-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="16d9c-133">Por exemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="16d9c-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="16d9c-134">Para problemas comuns com o registro de dispositivos do Azure Active Directory, confira [perguntas frequentes sobre dispositivos](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="16d9c-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
