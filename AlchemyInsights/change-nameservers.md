---
title: Alterar nameservers
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818600"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Atualize os servidores de nomes do domínio para apontar para a Microsoft

Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.
  
Para configurar o domínio no Microsoft 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.
  
1. Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.
  
2. Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Salvar alterações.

Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes com qualquer registrador de domínios](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  