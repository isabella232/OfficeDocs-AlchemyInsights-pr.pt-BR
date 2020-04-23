---
title: Atualize seus nameservers de domínio para apontar para a Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719981"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="0767c-102">Atualize seus nameservers de domínio para apontar para a Microsoft</span><span class="sxs-lookup"><span data-stu-id="0767c-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="0767c-103">Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="0767c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="0767c-104">Para configurar seu domínio com a Microsoft, os nameservers em seus registradores precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0767c-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="0767c-105">Crie ou edite registros de servidor de nomes no seu registrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="0767c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="0767c-106">Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="0767c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="0767c-107">Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:</span><span class="sxs-lookup"><span data-stu-id="0767c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="0767c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0767c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="0767c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0767c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="0767c-110">Salvar alterações.</span><span class="sxs-lookup"><span data-stu-id="0767c-110">Save changes.</span></span>

<span data-ttu-id="0767c-111">Você também pode encontrar instruções detalhadas neste artigo: [alterar os nameservers para configurar o Microsoft 365 com qualquer registrador de domínios](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="0767c-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  