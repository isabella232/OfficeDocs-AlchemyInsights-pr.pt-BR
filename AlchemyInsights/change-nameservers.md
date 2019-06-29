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
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 148fbee1c14a8da6ede5ec5ccae90b1a4340ce32
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363065"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="e62b5-102">Atualize seus nameservers de domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="e62b5-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="e62b5-103">Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="e62b5-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e62b5-p101">Para configurar o domínio no Office 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="e62b5-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e62b5-106">Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="e62b5-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="e62b5-107">Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:</span><span class="sxs-lookup"><span data-stu-id="e62b5-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e62b5-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e62b5-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e62b5-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e62b5-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e62b5-110">Salvar alterações.</span><span class="sxs-lookup"><span data-stu-id="e62b5-110">Save changes.</span></span>

<span data-ttu-id="e62b5-111">Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes para configurar o Office 365 com qualquer registrador de domínios](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="e62b5-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  