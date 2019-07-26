---
title: Alterar nameservers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902917"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="ed01c-102">Atualize seus nameservers de domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="ed01c-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="ed01c-103">Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="ed01c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ed01c-p101">Para configurar o domínio no Office 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="ed01c-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ed01c-106">Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="ed01c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="ed01c-107">Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:</span><span class="sxs-lookup"><span data-stu-id="ed01c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ed01c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ed01c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ed01c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ed01c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ed01c-110">Salvar alterações.</span><span class="sxs-lookup"><span data-stu-id="ed01c-110">Save changes.</span></span>

<span data-ttu-id="ed01c-111">Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes para configurar o Office 365 com qualquer registrador de domínios](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="ed01c-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  