---
title: 2681 do simulador de ataque no Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713454"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="d47cc-102">Simulador de ataque no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d47cc-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="d47cc-103">Você está faltando no simulador de ataques?</span><span class="sxs-lookup"><span data-stu-id="d47cc-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="d47cc-104">O simulador de ataque requer o **office 365 Advanced Threat Protection Plan 2 (plano ATP 2)** ou o **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="d47cc-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="d47cc-105">O simulador de ataques **não** está incluído no Office 365 Advanced Threat Protection Plan 1 (plano ATP 1), Office 365 Enterprise E3 ou qualquer aplicativo do Microsoft 365 para assinaturas de negócios.</span><span class="sxs-lookup"><span data-stu-id="d47cc-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="d47cc-106">A conta que você usa para iniciar ataques simulados requer permissões de administrador global ou administrador de segurança e a autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="d47cc-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="d47cc-107">Para obter mais informações sobre os requisitos de simulador de ataques, consulte [Este tópico](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="d47cc-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="d47cc-108">Considerações importantes sobre simulações de ataque de **senha de força bruta** :</span><span class="sxs-lookup"><span data-stu-id="d47cc-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="d47cc-109">Se a conta de destino tiver a MFA habilitada e a senha tiver sido adivinhada corretamente, a conta não será mostrada como comprometida (o segundo fator de autenticação estará incompleto).</span><span class="sxs-lookup"><span data-stu-id="d47cc-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="d47cc-110">O arquivo de senha não pode ter mais de 10 MB.</span><span class="sxs-lookup"><span data-stu-id="d47cc-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="d47cc-111">Use uma senha por linha e inclua uma linha em branco (retorno de carro) após a última senha na lista.</span><span class="sxs-lookup"><span data-stu-id="d47cc-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="d47cc-112">Coisas importantes que você deve saber sobre as simulações de conexões de **spear phishing** :</span><span class="sxs-lookup"><span data-stu-id="d47cc-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="d47cc-113">Por design, você não pode fornecer um valor personalizado para a **URL do servidor de logon de phishing**.</span><span class="sxs-lookup"><span data-stu-id="d47cc-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="d47cc-114">Se um destinatário usar o [suplemento habilitar o relatório de mensagens](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) para relatar a mensagem como phishing, talvez você não receba alertas para a mensagem (pois esse é um ataque simulado).</span><span class="sxs-lookup"><span data-stu-id="d47cc-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="d47cc-115">Relatórios: após a conclusão do ataque simulado, você pode clicar em **detalhes do ataque** para ver o relatório.</span><span class="sxs-lookup"><span data-stu-id="d47cc-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="d47cc-116">Para obter instruções detalhadas e novos recursos no simulador de ataques, consulte [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="d47cc-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
