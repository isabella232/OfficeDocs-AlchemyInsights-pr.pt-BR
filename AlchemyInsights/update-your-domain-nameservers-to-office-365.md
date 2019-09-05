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
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742151"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="494e9-102">Atualize seus nameservers de domínio para o Office 365</span><span class="sxs-lookup"><span data-stu-id="494e9-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="494e9-103">Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="494e9-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="494e9-p101">Para configurar o domínio no Office 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="494e9-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="494e9-106">Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="494e9-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="494e9-107">Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:</span><span class="sxs-lookup"><span data-stu-id="494e9-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="494e9-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="494e9-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="494e9-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="494e9-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="494e9-110">Salvar alterações.</span><span class="sxs-lookup"><span data-stu-id="494e9-110">Save changes.</span></span>

<span data-ttu-id="494e9-111">Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes para configurar o Office 365 com qualquer registrador de domínios](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="494e9-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  