---
title: Migração do Proteção de Informações do Azure para rotular MIP/Unificado no Centro de Conformidade
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825359"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="d2221-102">Migração do Proteção de Informações do Azure para rotular MIP/Unificado no Centro de Conformidade</span><span class="sxs-lookup"><span data-stu-id="d2221-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="d2221-103">Para migrar de etiquetas do AIP para Rotulação Unificada no entro de Segurança e Conformidade, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d2221-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="d2221-104">**Ativar a proteção do portal do Azure**</span><span class="sxs-lookup"><span data-stu-id="d2221-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="d2221-105">Se você ainda não tiver feito isso, abra uma nova janela do navegador e [entre no portal do Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="d2221-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="d2221-106">Navegue até a lâmina **Proteção de Informações do Azure**.</span><span class="sxs-lookup"><span data-stu-id="d2221-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="d2221-107">Por exemplo, no menu Hub, clique em **Todos os serviços** e comece a digitar **Informações** na Caixa de filtro.</span><span class="sxs-lookup"><span data-stu-id="d2221-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="d2221-108">Selecione **Proteção de Informações do Azure**.</span><span class="sxs-lookup"><span data-stu-id="d2221-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="d2221-109">Se você ainda não tiver acessado a lâmina Proteção de Informações do Azure antes, confira [etapas adicionais](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) para adicionar essa lâmina ao Portal.</span><span class="sxs-lookup"><span data-stu-id="d2221-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="d2221-110">Para abrir a lâmina Proteção de Informações do Azure, você deve ter um [plano Premium de Proteção de Informações do Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ou um plano do Office 365 que inclui o Gerenciamento de Direitos.</span><span class="sxs-lookup"><span data-stu-id="d2221-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="d2221-111">Se você tem uma dessas assinaturas, mas vê uma mensagem informando que não foi possível encontrar uma assinatura válida, [contate o Suporte da Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ou usar seus canais de suporte padrão.</span><span class="sxs-lookup"><span data-stu-id="d2221-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="d2221-112">Localize as opções de menu **Gerenciar** e selecione **Ativação da proteção**.</span><span class="sxs-lookup"><span data-stu-id="d2221-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="d2221-113">Clique em **Ativar** e, em seguida, confirme a ação.</span><span class="sxs-lookup"><span data-stu-id="d2221-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="d2221-114">Quando a ativação estiver concluída, a barra de informações exibirá **Ativação concluída com sucesso**.</span><span class="sxs-lookup"><span data-stu-id="d2221-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="d2221-115">**Migrar os rótulos de Proteção de Informações do Azure para o Centro de Conformidade e Segurança do Office 365**</span><span class="sxs-lookup"><span data-stu-id="d2221-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="d2221-116">Verifique se você está conectado como um usuário com permissão de Administrador Global.</span><span class="sxs-lookup"><span data-stu-id="d2221-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="d2221-117">Navegue até a lâmina **Proteção de Informações do Azure**.</span><span class="sxs-lookup"><span data-stu-id="d2221-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="d2221-118">Na opção de menu **Gerenciar**, selecione **Rotulagem Unificada**.</span><span class="sxs-lookup"><span data-stu-id="d2221-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="d2221-119">Na lâmina **Proteção de Informações do Azure - Rotulação Unificada**, clique em **Ativar** e siga as instruções online.</span><span class="sxs-lookup"><span data-stu-id="d2221-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="d2221-120">**Observação**: Verifique se você tem as permissões apropriadas antes de ativar a Migração do Centro de Conformidade e Segurança.</span><span class="sxs-lookup"><span data-stu-id="d2221-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="d2221-121">Confira estes artigos para obter mais informações:</span><span class="sxs-lookup"><span data-stu-id="d2221-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="d2221-122">Você precisa ser um administrador global do para configurar a Proteção de Informações do Azure, ou posso delegar para outros administradores?</span><span class="sxs-lookup"><span data-stu-id="d2221-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="d2221-123">Informações importantes sobre funções administrativas depois da migração para o Centro de Conformidade e Segurança.</span><span class="sxs-lookup"><span data-stu-id="d2221-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="d2221-124">Para obter mais informações sobre o AIP para rotular a migração unificada para o Centro de Conformidade e Segurança, confira [Migrar rótulos](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="d2221-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
