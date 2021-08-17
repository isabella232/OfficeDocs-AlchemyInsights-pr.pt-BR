---
title: Criar uma captura de email de todos
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080734"
---
# <a name="create-an-email-catch-all"></a>Criar uma captura de email de todos

O uso de uma captura é fortemente desencorajado. É melhor fornecer um retorno para o remetente que permite que os remetentes saibam que sua mensagem não pôde ser entregue como endereçada para que eles possam tomar medidas. Você também pode limitar a caixa de correio monitorada para capturar apenas endereços de email anteriormente válidos. 

Qualquer captura de todas as caixas de correio receberá uma boa quantidade de spam e poderá, eventualmente, ser preenchida se não for monitorada de perto. (Há limites de recebimento.) 

Se você decidir prosseguir, siga estas etapas:

1. Crie um grupo dinâmico de distribuição & incluir "Todos os tipos de destinatários".

2. Crie uma Caixa de Correio dedicada para capturar emails, por exemplo, catchall@domain.com.

3. Para o domínio específico, de definir DomainType como "InternalRelay". Se você remover mais tarde a captura de todos, certifique-se de definir o domínio de volta como Autoritativo.

4. Crie uma Regra de Transporte de Fluxo de Email da seguinte forma:

    - Se o Remetente for "Fora da Organização"
    - Redirecionar a mensagem para Catchall@domain.com
    - Exceto se o destinatário for membro do allusers@domain.com (o Grupo de Distribuição contém todos os membros)
    - Certifique-se de validar se novas caixas de correio são adicionadas ao Grupo de Distribuição Dinâmica
