---
title: Criar um email capturar tudo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712974"
---
# <a name="create-an-email-catch-all"></a>Criar um email capturar tudo

O uso de um catch tudo é fortemente desencorajado. É melhor fornecer um repercussão para o remetente, permitindo que os remetentes saibam que a mensagem não puderam ser entregues conforme tratados, para que eles possam realizar ações. Você também pode limitar a caixa de correio monitorada para capturar apenas endereços de email válidos. 

Qualquer caixa de correio do catch receberá uma boa dose de spam e poderá, eventualmente, preencher se não estiver intimamente monitorado. (Há limites de recebimento.) 

Se você decidir continuar, siga estas etapas:

1. Criar um grupo dinâmico de distribuição & incluir "todos os tipos de destinatário."

2. Criar uma caixa de correio dedicada para capturar emails, por exemplo, catchall@domain.com.

3. Para o domínio específico, defina o DomainType como "InternalRelay". Se posteriormente você remover o catch, certifique-se de definir o domínio novamente como autoritativo.

4. Crie uma regra de transporte fluxo da seguinte maneira:

    - Se o remetente for "fora da organização"
    - Redirecionar a mensagem para o Catchall@domain.com
    - Exceto se o destinatário for um membro de allusers@domain.com (grupo de distribuição contém todos os membros)
    - Certifique-se de validar que novas caixas de correio são adicionadas ao grupo dinâmico de distribuição
