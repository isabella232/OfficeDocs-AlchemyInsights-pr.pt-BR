---
title: Conjunto de réplicas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110668"
---
# <a name="replica-set"></a>Conjunto de réplicas

O AADDS também é chamado como o domínio gerenciado. Na verdade, são dois controladores de domínio que são executados e mantidos pelo back-end. Os dois DCs incluem um DC principal e um DC de replicação. Backups no AADDS (domínio gerenciado) são um processo automatizado gerenciado pela plataforma do Azure. Em caso de um problema com seu domínio gerenciado, o suporte ao Azure pode ajudá-lo na restauração do backup.

Você cria cada conjunto de réplicas em uma rede virtual. Cada rede virtual deve ser igualada a todas as outras redes virtuais que hospedam o conjunto de réplicas de um domínio gerenciado. Essa configuração cria uma topologia de rede de malha que oferece suporte à replicação de diretório. Uma rede virtual pode dar suporte a vários conjuntos de réplicas, desde que cada conjunto de réplicas seja em uma sub-rede virtual diferente.

Para obter mais detalhes sobre o conjunto de réplicas, consulte [Conjuntos de réplicas de conceitos.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
