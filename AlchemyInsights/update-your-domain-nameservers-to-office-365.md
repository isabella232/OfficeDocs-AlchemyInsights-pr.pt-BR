---
title: Atualizar os servidores de nomes de domínio para o Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.openlocfilehash: 724e9f7501826dc238932ec08e8628d077e20e2c
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918423"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="a959c-102">Atualizar os servidores de nomes de domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="a959c-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="a959c-103">Observação: Alterações de servidor de nomes em alguns casos, podem demorar até 48 horas para propagar.</span><span class="sxs-lookup"><span data-stu-id="a959c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="a959c-p101">Para configurar o domínio no Office 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="a959c-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="a959c-106">Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="a959c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="a959c-107">Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:</span><span class="sxs-lookup"><span data-stu-id="a959c-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="a959c-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a959c-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="a959c-109">Ns2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a959c-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="a959c-110">Salvar alterações.</span><span class="sxs-lookup"><span data-stu-id="a959c-110">Save changes.</span></span>
    
<span data-ttu-id="a959c-111">Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes para configurar o Office 365 com qualquer registrador de domínios](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="a959c-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

