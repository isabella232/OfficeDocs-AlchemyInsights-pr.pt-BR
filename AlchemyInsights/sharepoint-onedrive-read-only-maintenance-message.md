---
title: Somente leitura para mensagem de manutenção ao tentar usar o SharePoint ou o OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051269"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="e1bd7-102">Somente leitura para mensagem de manutenção ao tentar usar o SharePoint ou o OneDrive</span><span class="sxs-lookup"><span data-stu-id="e1bd7-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="e1bd7-103">Os usuários podem receber uma mensagem **somente leitura para manutenção** ao tentar usar o SharePoint ou o onedrive para um dos cenários a seguir.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="e1bd7-104">Uma atividade de manutenção planejada ou ativa.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="e1bd7-105">Verifique se eles navegam para o [centro de mensagens](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="e1bd7-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="e1bd7-106">Um incidente de serviço ativo de alta prioridade que pode ocorrer.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="e1bd7-107">Verifique se há avisos/incidentes navegando até a [integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e1bd7-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="e1bd7-108">Um cenário de recuperação de reparo automático secundário que pode ocorrer devido a qualquer evento inesperado nos servidores que podem durar menos de 30 min.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="e1bd7-109">Não há postagens do centro de mensagens ou da integridade do serviço para essas pequenas recuperações, mas você deve voltar para o normal em breve.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="e1bd7-110">Em muito poucas ocasiões observamos que um dos três cenários listados acima tem sido a causa, e o serviço foi restaurado, mas o cache do navegador do usuário não foi apagado.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="e1bd7-111">Tente limpar o cache do navegador antes de navegar até o site.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="e1bd7-112">No navegador Microsoft Edge, selecione **configurações**e, em seguida, selecione **privacidade e segurança**.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="e1bd7-113">Em **limpar navegação**, selecione **escolher o que limpar**.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="e1bd7-114">Selecione **cookies e dados de sites salvos**e selecione **limpar**.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="e1bd7-115">Essas etapas podem diferir ao usar outros navegadores, como Mozilla Firefox ou Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="e1bd7-116">Outra opção seria abrir seu site do SharePoint ou o OneDrive em uma nova janela InPrivate.</span><span class="sxs-lookup"><span data-stu-id="e1bd7-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>