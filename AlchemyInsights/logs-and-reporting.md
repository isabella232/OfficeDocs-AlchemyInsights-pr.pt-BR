---
title: Logs e relatórios
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031492"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="52deb-102">Logs e relatórios</span><span class="sxs-lookup"><span data-stu-id="52deb-102">Logs and Reporting</span></span>

<span data-ttu-id="52deb-103">As perguntas frequentes sobre relatórios do [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) responderão a perguntas frequentes sobre os relatórios do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="52deb-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="52deb-104">Para saber mais, confira [relatórios do Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="52deb-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="52deb-105">**Solução de problemas com a Auditoria**</span><span class="sxs-lookup"><span data-stu-id="52deb-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="52deb-106">Se você estiver tendo problemas ao ver algumas atividades de auditoria e a Atividade ausente estiver [nessa](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)lista, protocole um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="52deb-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="52deb-107">Se você estiver tendo problemas ao ver os logs de auditoria em seu locatário, protocole um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="52deb-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="52deb-108">Se suas atividades de auditoria não aparecerem imediatamente no [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) Portal do Azure, confira nossas informações de latência e arquiva um tíquete de suporte se o atraso exceder a latência documentada.</span><span class="sxs-lookup"><span data-stu-id="52deb-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="52deb-109">Retenção de logs de atividades do Azure AD</span><span class="sxs-lookup"><span data-stu-id="52deb-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="52deb-110">Se você não vir toda a auditoria para o intervalo de datas selecionado, poderá baixar até 250 mil linhas (classificados pela mais recente) de logins do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="52deb-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="52deb-111">Para obter mais informações, consulte [o download de atividades de auditoria.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="52deb-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="52deb-112">**Solução de problemas com As insições**</span><span class="sxs-lookup"><span data-stu-id="52deb-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="52deb-113">Você só poderá ver os últimos 30 dias de dados se tiver uma licença do Azure AD Premium (P1 ou P2) para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="52deb-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="52deb-114">As assinaturas estão disponíveis apenas para locatários do Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="52deb-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="52deb-115">Ele não está disponível para locatários licenciados gratuitos ou básicos.</span><span class="sxs-lookup"><span data-stu-id="52deb-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="52deb-116">Se seu locatário tiver uma licença Premium P1 e você não [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) conseguir ver as insitções, confira nossas informações de latência e arquiva um tíquete de suporte se o atraso exceder a latência documentada.</span><span class="sxs-lookup"><span data-stu-id="52deb-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="52deb-117">Se você não vir todas as inscrições para o intervalo de datas selecionado, observe que você pode baixar até 250 mil linhas (classificados pelas mais recentes) de logins do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="52deb-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="52deb-118">Para obter mais informações, [consulte o download de atividades de login.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="52deb-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="52deb-119">**Solucionar problemas de relatórios de segurança (usuários sinalizados em risco, login arriscado)**</span><span class="sxs-lookup"><span data-stu-id="52deb-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="52deb-120">Usuários sinalizados para relatório de segurança de risco</span><span class="sxs-lookup"><span data-stu-id="52deb-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="52deb-121">Relatório de logins arriscados no portal do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="52deb-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="52deb-122">Eventos de risco do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="52deb-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
