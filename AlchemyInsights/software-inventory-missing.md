---
title: O inventário de software está ausente ou impreciso
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: 191d6ae772dc1b1c6b15071da9c4aca14429cf2db17be6ee0db6b23ea0d29e2d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084631"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>O inventário de software está ausente ou impreciso

O inventário de software no TVM (gerenciamento de ameaças e vulnerabilidades) é uma lista de softwares conhecidos da organização com as CPE (Enumerações de Plataforma Comum) oficiais.

Os produtos de software sem uma CPE oficial não têm vulnerabilidades publicadas. O inventário também inclui detalhes, como o nome do fornecedor, o número de fraquezas, as ameaças e o número de dispositivos expostos.

As alterações de software nos dispositivos geralmente são refletidas em portais de segurança dentro de duas horas. No entanto, às vezes isso pode levar mais tempo. Atualmente, não há nenhuma maneira de forçar uma sincronização; essa é uma avaliação contínua.

Se você fez uma alteração de software e a alteração não for refletida com precisão no TVM após 5 horas, siga estas etapas:

1. Verifique a seção de evidências do software para entender como o software foi detectado.
1. Certifique-se de que o software tem suporte. O software pode estar visível apenas no nível do dispositivo, mesmo que atualmente não tenha suporte para o gerenciamento de ameaças e vulnerabilidades. No entanto, apenas dados limitados estão disponíveis.
1. Para ver as etapas para relatar a imprecisão do portal, confira [Relatar imprecisão](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Observação**: relatar uma imprecisão do portal MDE é um canal unidirecional da engenharia. Se o problema for urgente, abra um tíquete de suporte.

Para saber mais, confira [Inventário de software – gerenciamento de ameaças e vulnerabilidades](/microsoft-365/security/defender-endpoint/tvm-software-inventory).