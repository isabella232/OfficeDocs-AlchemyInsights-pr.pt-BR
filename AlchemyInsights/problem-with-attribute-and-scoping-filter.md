---
title: Problemas com o filtro de atributo e o de escopo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430710"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="24622-102">Problemas com o filtro de atributo e o de escopo</span><span class="sxs-lookup"><span data-stu-id="24622-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="24622-103">**Problema com valores UPN conflitantes**</span><span class="sxs-lookup"><span data-stu-id="24622-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="24622-104">O Workday para o AD User Provisioning Workday to AD User Provisioning mostra a mensagem de erro **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="24622-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="24622-105">A operação falhou porque o valor UPN fornecido para adição/modificação não é exclusivo para toda a floresta.</span><span class="sxs-lookup"><span data-stu-id="24622-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="24622-106">Detalhes do Erro: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="24622-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="24622-107">O valor **userPrincipalName** que o conector Workday tenta definir ao criar a conta de usuário do AD já existe no domínio do AD de destino.</span><span class="sxs-lookup"><span data-stu-id="24622-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="24622-108">Isso implica que (1) o usuário já existe e a verificação de ID correspondente falhou para o usuário ou (2) a regra de geração de UPN gerou um valor conflitante.</span><span class="sxs-lookup"><span data-stu-id="24622-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="24622-109">Veja as etapas de resolução sugeridas:</span><span class="sxs-lookup"><span data-stu-id="24622-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="24622-110">Se o usuário já existe e a verificação de ID correspondente não conseguiu vincular a conta Workday à conta do Active Directory, então verifique se o atributo do ID correspondente (geralmente, **employeeID**) no Workday e no AD têm uma correspondência exata.</span><span class="sxs-lookup"><span data-stu-id="24622-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="24622-111">Se eles não corresponderem, será necessário corrigir algum problema existente nos dados.</span><span class="sxs-lookup"><span data-stu-id="24622-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="24622-112">Por exemplo, se o EmployeeID no Workday for 001052, e no AD for 1052, então o mecanismo de provisionamento falhará ao vincular as duas contas e tentará criar um usuário já existente.</span><span class="sxs-lookup"><span data-stu-id="24622-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="24622-113">A solução neste caso é alterar o valor **EmployeeID** no AD para incluir os zeros à esquerda e deixá-lo como 001052.</span><span class="sxs-lookup"><span data-stu-id="24622-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="24622-114">Se a expressão geradora de UPN não gerar um valor exclusivo, considere o uso da função de eliminação de duplicação **SelectUniqueValue** para gerar um valor exclusivo a cada vez.</span><span class="sxs-lookup"><span data-stu-id="24622-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="24622-115">**O Workday para o AD User Provisioning não define o valor do atributo gerente para a conta de usuário do AD**</span><span class="sxs-lookup"><span data-stu-id="24622-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="24622-116">O Workday para o trabalho do AD User Provisioning não define o valor do atributo **manager** para as contas de usuários do AD.</span><span class="sxs-lookup"><span data-stu-id="24622-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="24622-117">Há dois cenários possíveis quando esse comportamento acontece:</span><span class="sxs-lookup"><span data-stu-id="24622-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="24622-118">O gerenciador no Workday não pode ser resolvido para uma conta de usuário do AD correspondente, pois o gerenciador não está no escopo.</span><span class="sxs-lookup"><span data-stu-id="24622-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="24622-119">Em um cenário de **vários domínios do AD**, o gerenciador no Workday não está presente no mesmo domínio que o usuário.</span><span class="sxs-lookup"><span data-stu-id="24622-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="24622-120">Tente seguir estas etapas para resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="24622-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="24622-121">Se você definiu os filtros de escopo, verifique primeiro se o gerenciador está no escopo e se ele atende a cláusula de escopo.</span><span class="sxs-lookup"><span data-stu-id="24622-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="24622-122">Se o gerenciador não atender ao filtro de escopo, altere o filtro para que o gerenciador também esteja no escopo da operação de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="24622-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="24622-123">Se você tiver vários domínios do AD, o conector terá uma limitação conhecida como a incapacidade de resolver referências do gerenciador de domínios cruzados.</span><span class="sxs-lookup"><span data-stu-id="24622-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="24622-124">Para obter mais detalhes sobre como configurar o Workday para provisionamento automatizado, confira [Tutorial: Configurar o Workday para provisionamento automático](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="24622-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













