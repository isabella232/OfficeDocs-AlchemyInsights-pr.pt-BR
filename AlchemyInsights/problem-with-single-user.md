---
title: Problema com um único usuário
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428505"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="6b29b-102">Problema com um único usuário</span><span class="sxs-lookup"><span data-stu-id="6b29b-102">Problem with single user</span></span>

- <span data-ttu-id="6b29b-103">O usuário pode não ter sido provisionado porque o serviço ainda não teve a chance de avaliar o usuário.</span><span class="sxs-lookup"><span data-stu-id="6b29b-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="6b29b-104">Revise as diretrizes de quanto tempo o provisionamento leva, bem como a barra de progresso na página de configuração de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="6b29b-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="6b29b-105">Se o estado estável especificado na seção de detalhes adicionais for antes da data em que o usuário foi criado/atualizado/excluído, isso significa que ainda não avaliamos o usuário.</span><span class="sxs-lookup"><span data-stu-id="6b29b-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="6b29b-106">Nesse cenário, o melhor a fazer é aguardar o fim do serviço de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="6b29b-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="6b29b-107">Observe que nosso serviço só está ciente das alterações em um usuário no sistema de origem (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="6b29b-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="6b29b-108">Deve haver uma alteração válida no sistema de origem do Azure AD para detectar a alteração e fluí-la para o Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6b29b-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="6b29b-109">O serviço de provisionamento avaliou o usuário e determinou que ele não deve ser provisionado:</span><span class="sxs-lookup"><span data-stu-id="6b29b-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="6b29b-110">Se você tiver definido um filtro de scoping baseado em atributo, verifique se o usuário atende aos critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="6b29b-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="6b29b-111">Se os usuários já existirem no sistema de destino e no estado do usuário na origem e na combinação de destino, não tomaremos mais nenhuma ação.</span><span class="sxs-lookup"><span data-stu-id="6b29b-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="6b29b-112">O serviço de provisionamento tentou provisionar o usuário e falhou.</span><span class="sxs-lookup"><span data-stu-id="6b29b-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="6b29b-113">Para esses cenários, revise a guia solução de problemas e recomendações dos logs de provisionamento:</span><span class="sxs-lookup"><span data-stu-id="6b29b-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="6b29b-114">Um atributo necessário no usuário pode estar ausente no Active Directory local ou no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6b29b-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="6b29b-115">Por exemplo, as regras de geração userPrincipalName ou sAMAccountName não estão gerando o valor certo.</span><span class="sxs-lookup"><span data-stu-id="6b29b-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="6b29b-116">O atributo matching (geralmente employeeId) não está sendo resolvido para um usuário exclusivo no Active Directory local ou no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6b29b-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="6b29b-117">Por exemplo, há dois usuários com o mesmo employeeId no AD e o serviço retorna um código de erro indicando entradas de destino duplicadas para a mesma entrada de origem.</span><span class="sxs-lookup"><span data-stu-id="6b29b-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="6b29b-118">Para revisar logs para um único usuário e grupos, consulte [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="6b29b-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
