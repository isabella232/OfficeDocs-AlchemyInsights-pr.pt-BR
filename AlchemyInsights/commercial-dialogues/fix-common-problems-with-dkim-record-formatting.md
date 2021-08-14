---
title: Corrigir problemas comuns com formatação de registro DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930049"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Corrigir problemas comuns com formatação de registro DKIM

A maioria dos problemas de configuração de DKIM está relacionada a registros DNS incorretos.

Para corrigir os problemas de configuração do DKIM, verifique se o registro CNAME DKIM **(não** um registro TXT) está formatado corretamente. Para obter mais informações, consulte [O que você precisa fazer para configurar manualmente o DKIM em Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Se você precisar de ajuda com registros DNS em geral, consulte [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Depois de criar ou atualizar seus registros DNS DKIM no serviço de hospedagem DNS do seu domínio, você precisará aguardar a propagação dos registros DNS.
