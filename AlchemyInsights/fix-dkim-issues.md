---
title: Corrigir problemas de instalação do DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945919"
---
# <a name="fix-dkim-setup-issues"></a>Corrigir problemas de instalação do DKIM

Se você tiver problemas para habilitear o DKIM para seu domínio personalizado, use as seguintes etapas:

- A maioria dos problemas de instalação do DKIM está relacionada a registros DNS incorretos. Verifique se o registro CNAME do DKIM (**não** um registro TXT) está formatado corretamente. Para obter mais informações, consulte este [tópico](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Depois de criar ou atualizar seus registros DNS DKIM no serviço de hospedagem DNS do seu domínio (normalmente, seu registrador de domínios), aguarde até que os registros DNS se propaguem.

- Se você não puder criar os registros DNS DKIM no centro de administração, poderá substituir por seu domínio personalizado (por exemplo, contoso.com) e executar esse comando no \<CustomDomain\> [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
