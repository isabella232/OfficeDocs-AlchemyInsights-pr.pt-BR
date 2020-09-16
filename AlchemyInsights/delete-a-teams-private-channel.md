---
title: Excluir um canal privado do Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730903"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="4526d-102">Excluir um canal privado do Teams</span><span class="sxs-lookup"><span data-stu-id="4526d-102">Delete a Teams private channel</span></span>

<span data-ttu-id="4526d-103">A Microsoft está ciente de um problema ao excluir um canal privado do Teams, caso você tenha Políticas de Retenção do SharePoint habilitadas para o site do SharePoint subjacente.</span><span class="sxs-lookup"><span data-stu-id="4526d-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="4526d-104">A Microsoft está trabalhando em uma correção.</span><span class="sxs-lookup"><span data-stu-id="4526d-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="4526d-105">Enquanto isso, você pode usar as seguintes soluções alternativas para excluir o canal privado:</span><span class="sxs-lookup"><span data-stu-id="4526d-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="4526d-106">**Exclua a coleção do Team/site da política de retenção do SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="4526d-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="4526d-107">Vá para o portal de administração do Office 365 e selecione **Mostrar todos** no painel de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="4526d-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="4526d-108">Em **Centros de Administração**, vá para **Segurança e Conformidade** > **Prevenção de Perda de Dados** > **Política**.</span><span class="sxs-lookup"><span data-stu-id="4526d-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="4526d-109">Identifique qualquer política que se aplica aos sites do SharePoint, e modifique a política de modo que o site do SharePoint para o Team que contém o canal privado NÃO esteja incluído na política de retenção.</span><span class="sxs-lookup"><span data-stu-id="4526d-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="4526d-110">Salvar a política.</span><span class="sxs-lookup"><span data-stu-id="4526d-110">Save the policy.</span></span>
    <span data-ttu-id="4526d-111">Pode levar até 24 horas para as configurações de política terem efeito.</span><span class="sxs-lookup"><span data-stu-id="4526d-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="4526d-112">Depois que o site tiver sido excluído, você poderá excluir o canal privado.</span><span class="sxs-lookup"><span data-stu-id="4526d-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="4526d-113">Você ***pode*** ser capaz de excluir o canal privado usando o Microsoft Teams em seu dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="4526d-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="4526d-114">Para informações relacionadas ao SharePoint, confira [Não é possível excluir itens no SharePoint Online ou no OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="4526d-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>