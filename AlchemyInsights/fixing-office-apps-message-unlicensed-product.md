---
title: Não é possível ativar o Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798668"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="e4579-102">Não é possível ativar o Office</span><span class="sxs-lookup"><span data-stu-id="e4579-102">Unable to activate Office</span></span>

<span data-ttu-id="e4579-103">**Observação**: se você estiver usando uma versão mais antiga do Windows (Por exemplo, Windows 7), certifique-se de que o TLS 1.2 está habilitado como padrão.</span><span class="sxs-lookup"><span data-stu-id="e4579-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="e4579-104">Para obter mais informações, confira [Atualizar para habilitar o TLS 1.1 e o TLS 1.2 como protocolos seguros padrão em WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="e4579-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="e4579-105">Verifique se o status da sua assinatura expirou.</span><span class="sxs-lookup"><span data-stu-id="e4579-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="e4579-106">Certifique-se de ter uma assinatura que permita licenças de cliente, como o Office 365 Business ou Business Premium, e [garanta que o usuário tenha uma licença atribuída](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="e4579-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="e4579-107">Certifique-se de que o usuário esteja entrando no Office com a mesma conta para a qual a assinatura foi atribuída.</span><span class="sxs-lookup"><span data-stu-id="e4579-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e4579-108">Verifique a [página de integridade do serviço do Office 365](/office365/enterprise/view-service-health) para ver se há algum problema conhecido com o serviço.</span><span class="sxs-lookup"><span data-stu-id="e4579-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e4579-p102">Verifique o firewall, software antivírus e as configurações do proxy para confirmar se eles não estão bloqueando o acesso dos aplicativos Microsoft 365 à Internet. Confira os [URLs do Office 365 e os intervalos de endereços IP](/office365/enterprise/urls-and-ip-address-ranges "Intervalos de endereços IP e URLs do Office 365").</span><span class="sxs-lookup"><span data-stu-id="e4579-p102">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet. Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="e4579-111">**Dica** em computadores com Windows, podemos diagnosticar e corrigir automaticamente vários problemas de entrada comuns do Office para você.</span><span class="sxs-lookup"><span data-stu-id="e4579-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="e4579-112">Baixe e execute o  **[Assistente de Suporte e Recuperação da Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para usar nossa ferramenta automatizada.</span><span class="sxs-lookup"><span data-stu-id="e4579-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="e4579-113">Siga estas instruções para solucionar o problema:</span><span class="sxs-lookup"><span data-stu-id="e4579-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="e4579-114">Abra um aplicativo do Office e [saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) das contas de usuários existentes.</span><span class="sxs-lookup"><span data-stu-id="e4579-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e4579-115">[Remova](/microsoft-365/admin/manage/remove-licenses-from-users) e [reatribua](/microsoft-365/admin/manage/assign-licenses-to-users) a licença do Office e, em seguida, [entre no Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.</span><span class="sxs-lookup"><span data-stu-id="e4579-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e4579-116">Execute a [Solução de Problemas de Ativação](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="e4579-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="e4579-117">Reinicie o estado de ativação do Office</span><span class="sxs-lookup"><span data-stu-id="e4579-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reiniciar o estado de ativação do Office")
- [<span data-ttu-id="e4579-118">Execute um Reparo Online do Office</span><span class="sxs-lookup"><span data-stu-id="e4579-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="e4579-119">Para mais opções de solução de problemas, confira:</span><span class="sxs-lookup"><span data-stu-id="e4579-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="e4579-120">Erros de ativação e de Produto Não Licenciado no Office</span><span class="sxs-lookup"><span data-stu-id="e4579-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="e4579-121">Erro "Não foi possível conectar-se à sua conta. Tente novamente mais tarde" ao ativar o Office</span><span class="sxs-lookup"><span data-stu-id="e4579-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)