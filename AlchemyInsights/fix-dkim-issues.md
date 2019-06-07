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
# <a name="fix-dkim-setup-issues"></a>Corrigir problemas de configuração do DKIM

Se você tiver problemas ao habilitar o DKIM para o seu domínio personalizado, siga estas etapas:

- A maioria dos problemas de instalação do DKIM está relacionada a registros DNS incorretos. Verifique se o registro CNAME DKIM (**não** um registro txt) está formatado corretamente. Para obter mais informações, consulte este [tópico](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Depois de criar ou atualizar seus registros DNS do DKIM no serviço de hospedagem DNS do seu domínio (normalmente, seu registrador de domínio), aguarde até que os registros DNS se propaguem.

- Se não for possível criar os registros DNS do DKIM no centro de administração, você \<poderá\> substituir o CustomDomain pelo seu domínio personalizado (por exemplo, contoso.com) e executar este comando no PowerShell `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`do [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):.
