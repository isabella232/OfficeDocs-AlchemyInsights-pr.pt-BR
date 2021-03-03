---
title: Monitorar o Acesso Condicional do Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416919"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="dcb8d-102">Monitorar o Acesso Condicional do Intune</span><span class="sxs-lookup"><span data-stu-id="dcb8d-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="dcb8d-103">Os usuários direcionados com acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="dcb8d-104">Para resolver, recomendamos uma ou mais das seguintes soluções:</span><span class="sxs-lookup"><span data-stu-id="dcb8d-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="dcb8d-105">Se presume-se que o dispositivo está inscrito, aconselha o usuário a ir até o aplicativo Portal da Empresa e verificar se ele aparece no Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="dcb8d-106">Se não for, o usuário deverá registrar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="dcb8d-107">No portal do Azure, vá para **Conformidade do Dispositivo do Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="dcb8d-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="dcb8d-108">Para exibir o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como **compatível,** em **Monitor,** clique em Conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="dcb8d-109">No portal do Azure, vá para **Conformidade do Dispositivo do Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="dcb8d-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="dcb8d-110">Em **Gerenciar,** clique em **Políticas**.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="dcb8d-111">Na lista de políticas de conformidade, verifique se um perfil está atribuído ao dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="dcb8d-112">Se nenhum perfil for atribuído, o Intune não poderá confirmar o status de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="dcb8d-113">Edite a atribuição de acesso condicional do usuário.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="dcb8d-114">No portal do Azure, navegue até Políticas de acesso condicional do **Intune,** selecione uma política na lista e clique em  >    >  Usuários **e grupos.**</span><span class="sxs-lookup"><span data-stu-id="dcb8d-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="dcb8d-115">Para direcionar uma determinada política para alguém, adicione-a à lista **Incluir**.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="dcb8d-116">Para garantir que uma pessoa seja omitida da política, adicione-a à lista **Excluir**.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="dcb8d-117">**Links úteis:**</span><span class="sxs-lookup"><span data-stu-id="dcb8d-117">**Helpful links:**</span></span>

- [<span data-ttu-id="dcb8d-118">Visão geral da conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="dcb8d-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="dcb8d-119">Solução de problemas de CA</span><span class="sxs-lookup"><span data-stu-id="dcb8d-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="dcb8d-120">Política de solução de problemas</span><span class="sxs-lookup"><span data-stu-id="dcb8d-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="dcb8d-121">Monitorando a conformidade do dispositivo do Intune</span><span class="sxs-lookup"><span data-stu-id="dcb8d-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="dcb8d-122">Essas etapas só são úteis na solução de problemas do recurso do Azure Active Directory Acesso Condicional.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="dcb8d-123">Também é possível colocar em quarentena um dispositivo bloqueando o acesso de email com a política do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcb8d-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="dcb8d-124">Mais informações sobre o gerenciamento de dispositivos do Exchange podem ser encontradas [**aqui**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="dcb8d-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
