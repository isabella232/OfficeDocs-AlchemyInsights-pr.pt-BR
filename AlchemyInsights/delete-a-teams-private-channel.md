---
title: Excluir um canal privado do Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431295"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="b264a-102">Excluir um canal privado do Teams</span><span class="sxs-lookup"><span data-stu-id="b264a-102">Delete a Teams private channel</span></span>

<span data-ttu-id="b264a-103">A Microsoft está ciente de um problema ao excluir um canal privado do Teams, caso você tenha Políticas de Retenção do SharePoint habilitadas para o site do SharePoint subjacente.</span><span class="sxs-lookup"><span data-stu-id="b264a-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="b264a-104">A Microsoft está trabalhando em uma correção.</span><span class="sxs-lookup"><span data-stu-id="b264a-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="b264a-105">Enquanto isso, você pode usar as seguintes soluções alternativas para excluir o canal privado:</span><span class="sxs-lookup"><span data-stu-id="b264a-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="b264a-106">**Exclua a coleção do Team/site da política de retenção do SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="b264a-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="b264a-107">Vá para o portal de administração do Office 365 e selecione **Mostrar todos** no painel de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="b264a-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="b264a-108">Em **Centros de Administração**, vá para **Segurança e Conformidade** > **Prevenção de Perda de Dados** > **Política**.</span><span class="sxs-lookup"><span data-stu-id="b264a-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="b264a-109">Identifique qualquer política que se aplica aos sites do SharePoint, e modifique a política de modo que o site do SharePoint para o Team que contém o canal privado NÃO esteja incluído na política de retenção.</span><span class="sxs-lookup"><span data-stu-id="b264a-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="b264a-110">Salvar a política.</span><span class="sxs-lookup"><span data-stu-id="b264a-110">Save the policy.</span></span>
    <span data-ttu-id="b264a-111">Pode levar até 24 horas para as configurações de política terem efeito.</span><span class="sxs-lookup"><span data-stu-id="b264a-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="b264a-112">Depois que o site tiver sido excluído, você poderá excluir o canal privado.</span><span class="sxs-lookup"><span data-stu-id="b264a-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="b264a-113">Você ***pode*** ser capaz de excluir o canal privado usando o Microsoft Teams em seu dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="b264a-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="b264a-114">Para informações relacionadas ao SharePoint, confira [Não é possível excluir itens no SharePoint Online ou no OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="b264a-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>