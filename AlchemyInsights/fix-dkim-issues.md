---
title: Corrigir problemas de configuração do DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717550"
---
# <a name="fix-dkim-setup-issues"></a>Corrigir problemas de configuração do DKIM

Se você tiver problemas ao habilitar o DKIM para o seu domínio personalizado, siga estas etapas:

- A maioria dos problemas de instalação do DKIM está relacionada a registros DNS incorretos. Verifique se o registro CNAME DKIM (**não** um registro txt) está formatado corretamente. Para obter mais informações, consulte este [tópico](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Depois de criar ou atualizar seus registros DNS do DKIM no serviço de hospedagem DNS do seu domínio (normalmente, seu registrador de domínio), aguarde até que os registros DNS se propaguem.

- Se não for possível criar os registros DNS do DKIM no centro de administração, você \<poderá\> substituir o CustomDomain pelo seu domínio personalizado (por exemplo, contoso.com) e executar este comando no PowerShell `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`do [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):.
