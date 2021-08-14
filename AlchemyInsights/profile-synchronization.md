---
title: Sincronização de perfil
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923632"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando minhas alterações de perfil são sincronizadas com o aplicativo SharePoint Perfil de Usuário?

SharePoint Online usa o trabalho de timer de Importação do Active Directory (Importação de AD) para importar usuários e grupos para o Aplicativo de Perfil de Usuário. 
  
1. A Importação do AD sincroniza as alterações do SharePoint De diretório online para o Aplicativo de Perfil de Usuário. Essas alterações são processadas em lotes.
    
2. O trabalho de timer é executado até que as alterações sejam sincronizadas.
    
> [!NOTE]
> O tempo necessário para executar o trabalho depende do número de alterações no processo. Um grande número de alterações leva mais tempo. O Contrato de Nível de Serviço (SLA) afirma que uma alteração para um usuário no diretório SharePoint Online será refletida no Aplicativo de Perfil de Usuário em 24 horas. 
  
[Mais informações sobre a sincronização de perfil de usuário no SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

