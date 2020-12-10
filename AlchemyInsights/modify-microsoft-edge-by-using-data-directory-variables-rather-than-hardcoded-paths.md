---
title: Modificar o Microsoft Edge usando variáveis de diretório de dados em vez de caminhos codificados
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608813"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Modificar o Microsoft Edge usando variáveis de diretório de dados em vez de caminhos codificados

Por exemplo, no Windows, para armazenar os dados de perfil em dados de aplicativo local de um usuário, em vez de no local padrão, defina a política **UserDataDir** como **$ {local_app_data} \Edge\Profile**. 

Para saber mais, confira [criar variáveis de diretório de dados do usuário do Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).