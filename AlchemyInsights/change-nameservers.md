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
ms.openlocfilehash: 3f39bfc585e8b805424cb7ccac76f81e1b2bfda9dcd1367361fec6a668c545bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017768"
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
  