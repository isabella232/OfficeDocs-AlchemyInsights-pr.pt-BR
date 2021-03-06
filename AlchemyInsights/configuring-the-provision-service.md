---
title: Configurando o serviço provisionamento
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
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480742"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="7bb18-102">Configurando o serviço provisionamento</span><span class="sxs-lookup"><span data-stu-id="7bb18-102">Configuring the Provision service</span></span>

<span data-ttu-id="7bb18-103">Para que o provisionamento de usuário automatizado funcione, o Azure AD requer credenciais válidas que permitem que ele se conecte à API de Serviços Web do Workday.</span><span class="sxs-lookup"><span data-stu-id="7bb18-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="7bb18-104">Além disso, o botão Conexão de Teste no aplicativo Workday to AD User Provisioning também valida se ele é capaz de se conectar ao Agente de Provisionamento de Conexão do Azure AD associado ao Domínio do AD.</span><span class="sxs-lookup"><span data-stu-id="7bb18-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="7bb18-105">Se o portal do Azure estiver retornando um erro ao salvar as credenciais, siga as etapas recomendadas abaixo:</span><span class="sxs-lookup"><span data-stu-id="7bb18-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="7bb18-106">Confirme se você configurou a conta de usuário do Sistema de Integração do Workday conforme indicado na seção tutorial Configurar o usuário do sistema de integração [no Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="7bb18-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="7bb18-107">Confirme se o Serviço de Agente de Provisionamento do Azure AD Connect está em execução no servidor Windows local usando o Console de Gerenciamento de Serviços.</span><span class="sxs-lookup"><span data-stu-id="7bb18-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="7bb18-108">Você também pode verificar o status do agente no portal do Azure clicando no botão Exibir agentes locais.</span><span class="sxs-lookup"><span data-stu-id="7bb18-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="7bb18-109">Certifique-se de que você está inserindo o valor do campo "Nome do Usuário do Dia de Trabalho" usando o formato username@workday nome do locatário.</span><span class="sxs-lookup"><span data-stu-id="7bb18-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="7bb18-110">Se o nome do locatário do dia de trabalho estiver ausente, a autenticação workday falhará.</span><span class="sxs-lookup"><span data-stu-id="7bb18-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="7bb18-111">Se você estiver configurando a integração com o locatário de implementação do Workday, anote os horários de inatividade agendados do locatário do Workday.</span><span class="sxs-lookup"><span data-stu-id="7bb18-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="7bb18-112">Workday programou o tempo de inatividade para seus locatários de implementação nos finais de semana (geralmente de sexta à noite até sábado de manhã) e falhas de conectividade durante essa janela de tempo de inatividade é um problema conhecido que resolve automaticamente assim que os locatários de implementação estão novamente online.</span><span class="sxs-lookup"><span data-stu-id="7bb18-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="7bb18-113">Em casos raros, você também poderá ver esse erro se a senha do Usuário do Sistema de Integração for alterada devido à atualização do locatário ou se a conta estiver bloqueada ou expirada.</span><span class="sxs-lookup"><span data-stu-id="7bb18-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="7bb18-114">Verifique o status do usuário do Sistema de Integração com o administrador do Workday.</span><span class="sxs-lookup"><span data-stu-id="7bb18-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="7bb18-115">Para obter mais detalhes sobre como configurar o Workday para provisionamento automatizado, confira [Tutorial: Configurar o Workday para provisionamento automático](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="7bb18-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
