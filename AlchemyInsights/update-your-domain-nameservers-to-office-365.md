---
title: Atualize seus nameservers de domínio para o Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 2447a3300782204b32d3c47325e1e987f6168be7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506035"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="5d500-102">Atualize seus nameservers de domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="5d500-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="5d500-103">Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="5d500-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="5d500-p101">Para configurar o domínio no Office 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="5d500-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="5d500-106">Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="5d500-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="5d500-107">Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:</span><span class="sxs-lookup"><span data-stu-id="5d500-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="5d500-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5d500-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="5d500-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5d500-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="5d500-110">Salvar alterações.</span><span class="sxs-lookup"><span data-stu-id="5d500-110">Save changes.</span></span>

<span data-ttu-id="5d500-111">Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes para configurar o Office 365 com qualquer registrador de domínios](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="5d500-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  