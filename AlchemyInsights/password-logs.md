---
title: Registros de senha
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523078"
---
# <a name="password-logs"></a><span data-ttu-id="227a6-102">Registros de senha</span><span class="sxs-lookup"><span data-stu-id="227a6-102">Password logs</span></span>

<span data-ttu-id="227a6-103">**Estou tendo problemas para acessar os registros de auditoria de redefinição de senha**</span><span class="sxs-lookup"><span data-stu-id="227a6-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="227a6-104">Para solucionar problemas relacionados ao acesso aos logs de auditoria de redefinição de senha, execute a seguinte etapa:</span><span class="sxs-lookup"><span data-stu-id="227a6-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="227a6-105">Certifique-se de que você está autorizado a visualizar os logs de auditoria.</span><span class="sxs-lookup"><span data-stu-id="227a6-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="227a6-106">Apenas as seguintes funções são autorizadas:</span><span class="sxs-lookup"><span data-stu-id="227a6-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="227a6-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="227a6-107">Global administrator</span></span>
 - <span data-ttu-id="227a6-108">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="227a6-108">Security administrator</span></span>
 - <span data-ttu-id="227a6-109">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="227a6-109">Security reader</span></span>

<span data-ttu-id="227a6-110">**Quero ver todos os eventos de auditoria de redefinição de senha desde o momento inicial em que foi implantado**</span><span class="sxs-lookup"><span data-stu-id="227a6-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="227a6-111">Até 120.000 eventos de redefinição/registro de senha são armazenados nos relatórios dos últimos 30 dias.</span><span class="sxs-lookup"><span data-stu-id="227a6-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="227a6-112">Este limite máximo se aplica à IU quando estiver baixando o CSV.</span><span class="sxs-lookup"><span data-stu-id="227a6-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="227a6-113">1 milhão de eventos estão disponíveis por meio do Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="227a6-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="227a6-114">Para obter mais informações, consulte os links abaixo:</span><span class="sxs-lookup"><span data-stu-id="227a6-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="227a6-115">Eventos de autoatendimento de redefinição de senha a partit da API de Relatórios e Eventos do Azure AD</span><span class="sxs-lookup"><span data-stu-id="227a6-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="227a6-116">Como baixar eventos de registro de redefinição de senha rapidamente com o Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="227a6-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="227a6-117">**Quero entender mais sobre os recursos de relatório de redefinição de senha**</span><span class="sxs-lookup"><span data-stu-id="227a6-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="227a6-118">Verifique quem está se registrando ou redefinindo senhas com logs de auditoria de redefinição de senha do Microsoft Azure Active Directory no portal do Azure em **Usuários e grupos**.</span><span class="sxs-lookup"><span data-stu-id="227a6-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="227a6-119">Para obter mais informações, consulte os seguintes links:</span><span class="sxs-lookup"><span data-stu-id="227a6-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="227a6-120">Visão geral dos relatórios de redefinição de senha</span><span class="sxs-lookup"><span data-stu-id="227a6-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="227a6-121">Como visualizar os relatórios de redefinição de senha no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="227a6-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="227a6-122">Eventos de autoatendimento de redefinição de senha a partit da API de Relatórios e Eventos do Azure AD</span><span class="sxs-lookup"><span data-stu-id="227a6-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="227a6-123">Como baixar eventos de registro de redefinição de senha rapidamente com o Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="227a6-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


