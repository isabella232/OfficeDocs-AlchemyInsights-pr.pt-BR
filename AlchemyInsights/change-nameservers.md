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
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736637"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="52f18-102">Atualize seus nameservers de domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="52f18-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="52f18-103">Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="52f18-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="52f18-p101">Para configurar o domínio no Office 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="52f18-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="52f18-106">Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="52f18-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="52f18-107">Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:</span><span class="sxs-lookup"><span data-stu-id="52f18-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="52f18-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="52f18-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="52f18-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="52f18-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="52f18-110">Salvar alterações.</span><span class="sxs-lookup"><span data-stu-id="52f18-110">Save changes.</span></span>

<span data-ttu-id="52f18-111">Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes para configurar o Office 365 com qualquer registrador de domínios](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="52f18-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  