---
title: Sincronização de perfil
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274729"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando as alterações do meu perfil sincronizar o aplicativo de perfil de usuário do SharePoint?

SharePoint Online usa o trabalho de timer de importação do Active Directory (AD importar) para importar usuários e grupos para o aplicativo de perfil de usuário. 
  
1. Importação do AD sincroniza as alterações do repositório de diretório do SharePoint Online para o aplicativo de perfil de usuário. Essas alterações são processadas em lotes.
    
2. O trabalho de timer é executado até que as alterações são sincronizadas.
    
> [!NOTE]
> O tempo que leva para executar o trabalho depende do número de alterações para processar. Um grande número de alterações é mais demorado. O contrato de nível de serviço (SLA) afirma que uma alteração em um usuário no SharePoint Online Directory será refletida no aplicativo de perfil de usuário em 24 horas. 
  
[Mais informações sobre a sincronização de perfil do usuário no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

