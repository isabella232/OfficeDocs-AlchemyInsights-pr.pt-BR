---
title: Corrigir problemas de configuração do DKIM
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744938"
---
# <a name="fix-dkim-setup-issues"></a>Corrigir problemas de configuração do DKIM

Se você tiver problemas ao habilitar o DKIM para o seu domínio personalizado, siga estas etapas:

- A maioria dos problemas de instalação do DKIM está relacionada a registros DNS incorretos. Verifique se o registro CNAME DKIM (**não** um registro txt) está formatado corretamente. Para obter mais informações, consulte este [tópico](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Depois de criar ou atualizar seus registros DNS do DKIM no serviço de hospedagem DNS do seu domínio (normalmente, seu registrador de domínio), aguarde até que os registros DNS se propaguem.

- Se não for possível criar os registros DNS do DKIM no centro de administração, você poderá substituir \<CustomDomain\> pelo seu domínio personalizado (por exemplo, contoso.com) e executar este comando no [PowerShell do Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
