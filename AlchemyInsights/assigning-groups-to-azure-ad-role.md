---
title: Atribuindo grupos à função do Microsoft Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875330"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Atribuindo grupos à função do Microsoft Azure AD

Para atribuir um grupo do Microsoft Azure AD com a origem da autoridade no Microsoft Azure AD a uma função do Microsoft Azure AD, execute as seguintes etapas:

1. Crie um novo grupo - Para criar um novo grupo:

    a. Entre no centro de administração do Microsoft Azure AD com permissões de **administrador de função privilegiada** ou **administrador global**.
    b. Selecione **Azure Active Directory > Grupos > Todos os grupos > Novo grupo**.
    c. Crie o grupo.

2. Atribua a função ao grupo durante a criação do grupo ou após a criação do grupo.

    a. Para atribuir uma função ao grupo no momento da sua criação, altere as **funções do Microsoft Azure AD que podem ser atribuídas ao grupo** e crie o grupo.
    b. Para atribuir uma função ao grupo após sua criação, navegue até a guia **Funções atribuídas** para o grupo recém-criado e atribua a função ao grupo.  

**Gerenciar a associação de um grupo atribuído à função do Microsoft Azure AD**

Para evitar a elevação de privilégios, por padrão, apenas administradores com funções privilegiadas e administradores globais podem modificar a associação de um grupo que é atribuído a uma função. No entanto, eles podem escolher atribuir um proprietário a esse grupo e delegar essa tarefa.

Para obter mais detalhes sobre como atribuir grupos de nuvem a funções do Microsoft Azure AD, confira [Atribuir funções do AD ao grupo de nuvem](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Para obter mais detalhes sobre a solução de problemas de funções atribuídas a grupos de nuvem, confira [Solucionar problemas de funções atribuídas a grupos de nuvem](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





