---
title: Estou sendo bloqueado por Acesso Condicional com dispositivo associado ao domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965457"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="7c8b6-102">Estou sendo bloqueado por Acesso Condicional com dispositivo associado ao domínio</span><span class="sxs-lookup"><span data-stu-id="7c8b6-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="7c8b6-103">**Ferramentas altamente recomendadas**</span><span class="sxs-lookup"><span data-stu-id="7c8b6-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="7c8b6-104">[Ferramenta de Solução de Problemas de Registro de Dispositivos](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A ferramenta que ajuda a solucionar os problemas mais comuns de registro de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="7c8b6-105">[Script de teste de conectividade de registro de dispositivo ](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - O script que ajuda a garantir que um Dispositivo possa acessar pontos de extremidade de Registro de dispositivo na conta do sistema.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="7c8b6-106">[Script de limpeza de dispositivo do Azure Active Directory](https://github.com/mzmaili/AzureADDeviceCleanup) - O script que permite que você busque e gerencie dispositivos obsoletos em seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="7c8b6-107">Aqui estão alguns motivos comuns pelos quais o acesso condicional pode falhar em um dispositivo que ingressou em um domínio (Azure Active Directory Híbrido).</span><span class="sxs-lookup"><span data-stu-id="7c8b6-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="7c8b6-108">**Não há Azure AD PRT no dispositivo** - Você precisa garantir que o dispositivo tenha o Token de Atualização Primária do Azure Active Directory (PRT).</span><span class="sxs-lookup"><span data-stu-id="7c8b6-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="7c8b6-109">Para obter mais informações sobre PRT, confira este [documento](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="7c8b6-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="7c8b6-110">Para verificar se você tem Azure Active Directory PRT, você pode executar o comando `dsregcmd/status` no dispositivo e verificar se “AzureAdPrt” é igual a “YES”.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="7c8b6-111">Se "AzureAdPrt" for "NÃO", verifique o seguinte:</span><span class="sxs-lookup"><span data-stu-id="7c8b6-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="7c8b6-112">**Se você tem um ambiente federado com AD FS e ele está inacessível nas redes domésticas de seus usuários**: neste caso, certifique-se de que seus pontos de extremidade "mesclados de usuário" estejam acessíveis a partir da extranet.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="7c8b6-113">Se o seu AD FS estiver atrás de uma VPN, certifique-se de que os usuários se conectem à VPN e façam login novamente no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="7c8b6-114">Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="7c8b6-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="7c8b6-115">**Se o TPM do dispositivo está com defeito e, portanto, não pode autenticar o dispositivo**: Verifique "tpm.msc" para ver se o estado do TPM é "Pronto".</span><span class="sxs-lookup"><span data-stu-id="7c8b6-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="7c8b6-116">Caso contrário, execute `dsregcmd/leave` e deixe o dispositivo se reintegrar ao Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="7c8b6-117">Em seguida, tente novamente.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-117">Then, try again.</span></span> <span data-ttu-id="7c8b6-118">Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="7c8b6-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="7c8b6-119">**Você está usando um provedor de identidade de terceiros, que não oferece suporte ao protocolo WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="7c8b6-120">Conforme descrito em nossos documentos, os dispositivos híbridos associados ao Azure Active Directory não podem funcionar neste caso.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="7c8b6-121">Trabalhe com seu provedor de identidade para obter suporte.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="7c8b6-122">**Os usuários estão usando o navegador Chrome sem as contas do Windows 10** ou **extensão do Office O Chrome não usa automaticamente o PRT em dispositivos AAD ou híbridos AAD**: Isso leva à falha de qualquer políticas de Acesso Condicional baseadas no dispositivo, com a mensagem de erro “Dispositivo não registrado” exibida.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="7c8b6-123">Para usar o navegador Chrome corretamente, você deve instalar as “Contas do Windows 10” ou "extensão do Office para o navegador Chrome dos usuários" via SCCM ou Intune.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="7c8b6-124">Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="7c8b6-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="7c8b6-125">Se não for possível enviar a extensão remotamente, notifique os usuários para instalar manualmente uma das extensões acima para acessar aplicativos por meio de Acesso Condicional baseado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="7c8b6-126">Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="7c8b6-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="7c8b6-127">**O dispositivo foi corretamente ingressado no Azure AD híbrido, mas foi inadvertidamente excluído ou desabilitado, devido a alterações de sincronização no Azure AD Connect ou no portal do Azure**: Se isso acontecer, o objeto de dispositivo não será mais reconhecido como um dispositivo totalmente unido, embora os status "AzureAdJoined" e "PRT" apareçam como válidos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="7c8b6-128">Para corrigir esse problema, execute `dsregcmd/leave` nos dispositivos afetados e deixe-os reingressar no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="7c8b6-129">Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="7c8b6-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="7c8b6-130">Se seus dispositivos estiverem no Windows 10, atualização 1809, com VPN/Cloud Proxy e virem problemas com o estado "AzureAdPrt" ou qualquer aplicativo com problema de SSO (perspectiva de não conectar à caixa de correio mesmo que você tenha PRT), certifique-se de ter este patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ou atualização cumulativa de abril [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) para evitar falhas de PRT nessas máquinas.</span><span class="sxs-lookup"><span data-stu-id="7c8b6-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















