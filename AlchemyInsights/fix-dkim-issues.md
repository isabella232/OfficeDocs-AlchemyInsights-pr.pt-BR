---
title: Corrigir problemas de configuração do DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764823"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="1fbc9-102">Corrigir problemas de configuração do DKIM</span><span class="sxs-lookup"><span data-stu-id="1fbc9-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="1fbc9-103">Se você tiver problemas ao habilitar o DKIM para o seu domínio personalizado, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="1fbc9-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="1fbc9-104">A maioria dos problemas de instalação do DKIM está relacionada a registros DNS incorretos.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="1fbc9-105">Verifique se o registro CNAME DKIM (**não** um registro txt) está formatado corretamente.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="1fbc9-106">Para obter mais informações, consulte este [tópico](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="1fbc9-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="1fbc9-107">Depois de criar ou atualizar seus registros DNS do DKIM no serviço de hospedagem DNS do seu domínio (normalmente, seu registrador de domínio), aguarde até que os registros DNS se propaguem.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="1fbc9-108">Se não for possível criar os registros DNS do DKIM no centro de administração, você \<poderá\> substituir o CustomDomain pelo seu domínio personalizado (por exemplo, contoso.com) e executar este comando no PowerShell `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`do [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
