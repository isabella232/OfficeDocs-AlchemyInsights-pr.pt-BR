---
title: Alterar nameservers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714676"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="91990-102">Atualize os servidores de nomes do domínio para apontar para a Microsoft</span><span class="sxs-lookup"><span data-stu-id="91990-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="91990-103">Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.</span><span class="sxs-lookup"><span data-stu-id="91990-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="91990-p101">Para configurar o domínio no Microsoft 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.</span><span class="sxs-lookup"><span data-stu-id="91990-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="91990-106">Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.</span><span class="sxs-lookup"><span data-stu-id="91990-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="91990-107">Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:</span><span class="sxs-lookup"><span data-stu-id="91990-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="91990-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="91990-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="91990-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="91990-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="91990-110">Salvar alterações.</span><span class="sxs-lookup"><span data-stu-id="91990-110">Save changes.</span></span>

<span data-ttu-id="91990-111">Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes com qualquer registrador de domínios](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="91990-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  