---
title: Atualize os servidores de nomes do domínio para apontar para a Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734899"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Atualize os servidores de nomes do domínio para apontar para a Microsoft

Observação: às vezes, as alterações de nameserver podem levar até 48 horas para serem propagadas.
  
Para configurar seu domínio com a Microsoft, os nameservers em seus registradores precisam ser atualizados. Crie ou edite registros de servidor de nomes no seu registrador de domínio.
  
1. Acesse o site do registrador do domínio e localize a área em que você pode editar os servidores de nomes.

2. Criar ou editar dois registros de servidor de nomes para corresponder a estes valores:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Salvar alterações.

Você também pode encontrar instruções detalhadas neste artigo: [alterar os nameservers para configurar o Microsoft 365 com qualquer registrador de domínios](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  