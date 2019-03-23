---
title: Atualizar registros DNS para manter seu site com seu provedor de hospedagem atual
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30760974"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="42c67-102">Atualizar registros DNS para manter seu site com seu provedor de hospedagem atual</span><span class="sxs-lookup"><span data-stu-id="42c67-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="42c67-103">Na página [Domínios](https://portal.office.com/adminportal/home#/Domains), selecione o domínio que você usa para o site na lista de domínios e selecione **Configurações de DNS**, no Painel Gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="42c67-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="42c67-104">Selecione **+ Novo registro personalizado** e insira o seguinte:</span><span class="sxs-lookup"><span data-stu-id="42c67-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="42c67-105">Para **Tipo DNS**, insira: **A (Endereço)**</span><span class="sxs-lookup"><span data-stu-id="42c67-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="42c67-106">Para **Nome do host ou Alias**, digite o seguinte: **@**</span><span class="sxs-lookup"><span data-stu-id="42c67-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="42c67-107">Para o **Endereço IP**, digite o endereço IP estático no qual seu site está hospedado no momento (por exemplo, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="42c67-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="42c67-p101">Esse deve ser um endereço IP  *estático*  do site e não um endereço IP  *dinâmico*  . Verifique com o site o local de hospedagem do seu site para garantir que você pode obter um endereço IP estático para o site público.</span><span class="sxs-lookup"><span data-stu-id="42c67-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="42c67-110">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="42c67-110">Select **Save**.</span></span> 
    
<span data-ttu-id="42c67-111">Além disso, você pode criar um registro CNAME para ajudar os clientes a encontrarem seu site.</span><span class="sxs-lookup"><span data-stu-id="42c67-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="42c67-112">Selecione **+ Novo registro personalizado** e insira o seguinte:</span><span class="sxs-lookup"><span data-stu-id="42c67-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="42c67-113">Para **Tipo DNS**, insira: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="42c67-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="42c67-114">Para **Nome do host ou Alias**, digite: **www**</span><span class="sxs-lookup"><span data-stu-id="42c67-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="42c67-115">Em **Pontos de endereçamento**, digite o FQDN (nome de domínio totalmente qualificado) do seu site (por exemplo, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="42c67-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="42c67-116">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="42c67-116">Select **Save**.</span></span> 
    

