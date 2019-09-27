---
title: Local dos dados
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207249"
---
# <a name="data-location"></a><span data-ttu-id="269ca-102">Local dos dados</span><span class="sxs-lookup"><span data-stu-id="269ca-102">Data location</span></span>

<span data-ttu-id="269ca-103">Você pode exibir o local do seu locatário do Office 365 no centro de administração ou conectando-se ao Exchange Online por meio do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="269ca-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="269ca-104">**Centro de administração:**</span><span class="sxs-lookup"><span data-stu-id="269ca-104">**Admin center:**</span></span>
1. <span data-ttu-id="269ca-105">Faça logon no [centro de administração](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="269ca-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="269ca-106">Selecione **configurações** > **perfil da organização**.</span><span class="sxs-lookup"><span data-stu-id="269ca-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="269ca-107">Em **local dos dados**, selecione **Exibir detalhes**.</span><span class="sxs-lookup"><span data-stu-id="269ca-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="269ca-108">**™**</span><span class="sxs-lookup"><span data-stu-id="269ca-108">**PowerShell:**</span></span>
1. <span data-ttu-id="269ca-109">Conecte-se ao Exchange Online usando o Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="269ca-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="269ca-110">Execute o cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) para exibir uma lista das propriedades do locatário.</span><span class="sxs-lookup"><span data-stu-id="269ca-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="269ca-111">Observe a propriedade OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="269ca-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="269ca-112">Quando você tem o local de dados do EXO e do SPO, é possível determinar o local dos dados de outros serviços que você pode usar de [onde seus dados estão localizados](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="269ca-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>