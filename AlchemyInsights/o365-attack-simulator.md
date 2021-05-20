---
title: Simulador de Ataque 2681 no Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545714"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="ad489-102">Simulador de Ataque no Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ad489-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="ad489-103">Você está perdendo o Simulador de Ataque?</span><span class="sxs-lookup"><span data-stu-id="ad489-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="ad489-104">O Simulador de Ataque requer **o Microsoft Defender para Office 365 Plano 2** ou Office 365 Enterprise **E5**.</span><span class="sxs-lookup"><span data-stu-id="ad489-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="ad489-105">O **Simulador** de Ataque não está incluído no Microsoft Defender para Office 365 Plano 1, Office 365 Enterprise E3 ou qualquer assinatura Microsoft 365 Apps para Pequenos e Médios negócios.</span><span class="sxs-lookup"><span data-stu-id="ad489-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="ad489-106">A conta que você usa para iniciar ataques simulados requer permissões de administrador global ou administrador de segurança e autenticação multifafatória (MFA).</span><span class="sxs-lookup"><span data-stu-id="ad489-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="ad489-107">Para obter mais informações sobre os requisitos do Simulador de Ataque, [consulte este tópico](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="ad489-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="ad489-108">Coisas importantes a saber sobre **simulações** de ataque de Senha de Força Bruta:</span><span class="sxs-lookup"><span data-stu-id="ad489-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="ad489-109">Se a conta de destino tiver MFA habilitada e a senha tiver sido adivinhada corretamente, a conta não mostrará como comprometida (o segundo fator de autenticação estará incompleto).</span><span class="sxs-lookup"><span data-stu-id="ad489-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="ad489-110">O arquivo de senha não pode ser maior do que 10 MB.</span><span class="sxs-lookup"><span data-stu-id="ad489-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="ad489-111">Use uma senha por linha e inclua uma linha em branco (retorno de carro) após a última senha na lista.</span><span class="sxs-lookup"><span data-stu-id="ad489-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="ad489-112">Coisas importantes a saber sobre simulações de **anexação de Phishing** de Lança:</span><span class="sxs-lookup"><span data-stu-id="ad489-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="ad489-113">Por design, você não pode fornecer um valor personalizado para a URL do servidor **de logon de Phishing.**</span><span class="sxs-lookup"><span data-stu-id="ad489-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="ad489-114">Se um destinatário usar o complemento [Habilitar](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) a Mensagem de Relatório para relatar a mensagem como phishing, talvez você não receba alertas para a mensagem (porque é um ataque simulado).</span><span class="sxs-lookup"><span data-stu-id="ad489-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="ad489-115">Relatórios: depois que o ataque simulado for concluído, você poderá clicar em **Detalhes de** Ataque para ver o relatório.</span><span class="sxs-lookup"><span data-stu-id="ad489-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="ad489-116">Para obter instruções detalhadas e novos recursos no Simulador de Ataques, consulte [Simulador](/microsoft-365/security/office-365-security/attack-simulator)de Ataque em Microsoft 365 .</span><span class="sxs-lookup"><span data-stu-id="ad489-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
