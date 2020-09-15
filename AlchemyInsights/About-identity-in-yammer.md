---
title: Sobre identidades no Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664158"
---
# <a name="about-identity-in-yammer"></a>Sobre identidades no Yammer

É recomendável que todas as redes sigam as seguintes etapas para evitar problemas relacionados à identidade:

1. Impor identidade do Office 365 após provisionar contas da Microsoft 365 para usuários no Azure AD para garantir que todos os usuários entrem usando suas contas principais do Microsoft 365. Para mais informações, confira [Impor identidade do Office 365 para usuários do Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Consolidar várias redes do Yammer. As configurações herdadas do Yammer permitem que várias redes do Yammer sejam conectadas a um locatário. Para saber mais, confira [Migração de rede - Consolidar várias redes do Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opcionalmente, impor licenciamento do Yammer a bloquear usuários se eles não tiverem uma licença. Para saber mais, confira [Gerenciar licenças de usuário do Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Por fim, auditar a lista de usuários das redes antigas no Yammer e suspender usuários herdados. É recomendável suspender (desativar) usuários em vez de excluí-los pois a exclusão é irreversível. Para saber mais, confira [Auditar usuários do Yammer em redes conectadas ao Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [Remover usuários](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Ao configurar o Yammer seguindo essas etapas, você também poderá configurar sua rede no modo Nativo para Microsoft 365 no Yammer. Para saber mais, confira[Configurar sua rede no modo Nativo para Microsoft 365 no Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).