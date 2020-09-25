---
title: Não é possível ativar o Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: e052c18eae035ff05c70a223f6d8a2eab875b2c9
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236077"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="07b98-102">Não é possível ativar o Office</span><span class="sxs-lookup"><span data-stu-id="07b98-102">Unable to activate Office</span></span>

- <span data-ttu-id="07b98-103">Verifique se o status da sua assinatura expirou.</span><span class="sxs-lookup"><span data-stu-id="07b98-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="07b98-104">Certifique-se de ter uma assinatura que permita licenças de cliente, como o Office 365 Business ou Business Premium, e [garanta que o usuário tenha uma licença atribuída](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="07b98-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="07b98-105">Certifique-se de que o usuário esteja entrando no Office com a mesma conta para a qual a assinatura foi atribuída.</span><span class="sxs-lookup"><span data-stu-id="07b98-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="07b98-106">Verifique a [página de integridade do serviço do Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) para ver se há algum problema conhecido com o serviço.</span><span class="sxs-lookup"><span data-stu-id="07b98-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="07b98-107">Verifique as configurações de firewall, software antivírus e proxy para verificar se eles estão bloqueando o acesso de aplicativos do Microsoft 365 à Internet.</span><span class="sxs-lookup"><span data-stu-id="07b98-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="07b98-108">Confira [URLs e intervalos de endereços IP do Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Intervalos de endereços IP e URLs do Office 365").</span><span class="sxs-lookup"><span data-stu-id="07b98-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="07b98-109">**Dica** em computadores com Windows, podemos diagnosticar e corrigir automaticamente vários problemas de entrada comuns do Office para você.</span><span class="sxs-lookup"><span data-stu-id="07b98-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="07b98-110">Baixe e execute o  **[Assistente de Suporte e Recuperação da Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para usar nossa ferramenta automatizada.</span><span class="sxs-lookup"><span data-stu-id="07b98-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="07b98-111">Siga estas instruções para solucionar o problema:</span><span class="sxs-lookup"><span data-stu-id="07b98-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="07b98-112">Abra um aplicativo do Office e [saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) das contas de usuários existentes.</span><span class="sxs-lookup"><span data-stu-id="07b98-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="07b98-113">[Remova](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [reatribua](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a licença do Office e, em seguida, [entre no Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.</span><span class="sxs-lookup"><span data-stu-id="07b98-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="07b98-114">Execute a [Solução de Problemas de Ativação](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="07b98-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="07b98-115">Reinicie o estado de ativação do Office</span><span class="sxs-lookup"><span data-stu-id="07b98-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reiniciar o estado de ativação do Office")
- [<span data-ttu-id="07b98-116">Execute um Reparo Online do Office</span><span class="sxs-lookup"><span data-stu-id="07b98-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="07b98-117">Para mais opções de solução de problemas, confira:</span><span class="sxs-lookup"><span data-stu-id="07b98-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="07b98-118">Erros de ativação e de Produto Não Licenciado no Office</span><span class="sxs-lookup"><span data-stu-id="07b98-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="07b98-119">Erro "Não foi possível conectar-se à sua conta. Tente novamente mais tarde" ao ativar o Office</span><span class="sxs-lookup"><span data-stu-id="07b98-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)