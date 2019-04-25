---
title: Sincronização de perfil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371972"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando o meu perfil é alterado, sincronizar com o aplicativo de perfil de usuário do SharePoint?

O SharePoint Online usa o trabalho de timer de importação do Active Directory (AD Import) para importar usuários e grupos para o aplicativo de perfil de usuário. 
  
1. A importação do AD sincroniza as alterações do repositório de diretórios do SharePoint Online para o aplicativo de perfil de usuário. Essas alterações são processadas em lotes.
    
2. O trabalho de timer é executado até que as alterações sejam sincronizadas.
    
> [!NOTE]
> O tempo necessário para a execução do trabalho depende do número de alterações a serem processadas. Um grande número de alterações demora mais. O contrato de nível de serviço (SLA) informa que uma alteração em um usuário no diretório do SharePoint Online será refletida no aplicativo de perfil de usuário em 24 horas. 
  
[Mais informações sobre a sincronização de perfil de usuário no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

