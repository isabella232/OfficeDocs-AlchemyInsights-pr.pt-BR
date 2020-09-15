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
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Atualize os servidores de nomes do domínio para apontar para a Microsoft

Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.
  
Para configurar o domínio no Microsoft 365, os servidores de nomes no seu registrador precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.
  
1. Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.
  
2. Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Salvar alterações.

Você também pode encontrar instruções detalhadas neste artigo: [Alterar os servidores de nomes com qualquer registrador de domínios](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  