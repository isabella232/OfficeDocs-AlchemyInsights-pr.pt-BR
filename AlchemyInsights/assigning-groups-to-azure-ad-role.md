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
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036228"
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





