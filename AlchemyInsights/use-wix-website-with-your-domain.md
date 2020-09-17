---
title: Usando o site do Wix com domínios do Office 365 comprados ou gerenciados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: b45923ef112917fb95263dc2690672847129b05f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795043"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Usando o site do Wix com domínios do Office 365 comprados ou gerenciados

- [Atualize os registros DNS para manter seu site com seu provedor de hospedagem atual](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- O artigo do Wix "Conectando um Domínio ao Wix usando o Método Apontador" recomenda usar o ponteiro (adicionar registros DNS por meio do link acima), em vez de alterar os servidores de nomes ao usar o Office 365
- Se você escolher alterar os servidores de nomes para os da Wix, você deve  [Criar os registros DNS na Wix para a Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Se o seu domínio foi adquirido na Microsoft, os servidores de nomes não podem ser alterados. Se você precisar alterar os servidores de nomes, o domínio adquirido pela Microsoft deverá ser  [transferido para o outro provedor de hospedagem após 60 dias](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)