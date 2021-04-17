---
title: 'AIP: políticas que não se comportam como esperado'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821615"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="e8589-102">AIP: políticas que não se comportam como esperado</span><span class="sxs-lookup"><span data-stu-id="e8589-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="e8589-103">Proteção de Informações do Azure: para políticas que não se comportam como esperado, confira a seguir como obter diretrizes recomendadas para vários problemas de política:</span><span class="sxs-lookup"><span data-stu-id="e8589-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="e8589-104">Se você estiver tendo problemas com as marcações visuais, consulte [Quando as marcações visuais forem aplicadas](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="e8589-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="e8589-105">Se você estiver tendo problemas com a rotulagem automática, consulte [Como configurar condições para a classificação automática e recomendada da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [O que os tipos de informações confidenciais procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="e8589-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="e8589-106">Se você estiver tendo problemas com a proteção Nativo/Pfile, consulte [Configuração da API de arquivo](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="e8589-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="e8589-107">Verifique se você está usando políticas de escopo não configuradas corretamente: [Como configurar a política de Proteção de Informações do Azure para usuários específicos usando políticas de escopo](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="e8589-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="e8589-108">Se a rotulagem automática não estiver funcionando no Outlook ao anexar um documento rotulado, verifique se DRMEncryptProperty não está definido como descrito aqui: [Configurações de registro do IRM para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="e8589-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="e8589-109">Se você ainda estiver enfrentando problemas, colete os logs do cliente de Proteção de Informações do Azure e anexe os logs exportados a esse tíquete.</span><span class="sxs-lookup"><span data-stu-id="e8589-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="e8589-110">Abra um documento do Office ou crie um novo email no Outlook.</span><span class="sxs-lookup"><span data-stu-id="e8589-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="e8589-111">Clique em **Proteção/Confidencialidade** > **Ajuda e comentários**.</span><span class="sxs-lookup"><span data-stu-id="e8589-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="e8589-112">Clique em **Exportar Logs**.</span><span class="sxs-lookup"><span data-stu-id="e8589-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="e8589-113">Salve os logs no local desejado e anexe-os à esta solicitação de serviço.</span><span class="sxs-lookup"><span data-stu-id="e8589-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="e8589-114">Recursos adicionais:</span><span class="sxs-lookup"><span data-stu-id="e8589-114">Additional resources:</span></span>

- [<span data-ttu-id="e8589-115">Como configurar um rótulo para marcações visuais da Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="e8589-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="e8589-116">Analisar a documentação da Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="e8589-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="e8589-117">Usar rótulos de confidencialidade em aplicativos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e8589-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

