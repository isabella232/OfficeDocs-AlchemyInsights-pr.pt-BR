---
title: Modifique o Microsoft Edge usando variáveis de diretório de dados em vez de caminhos codificados
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: e3ad930ec79ef82f3bf95e84cb88e8bb9aea13637d8e59d845b486604664b137
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53992279"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Modifique o Microsoft Edge usando variáveis de diretório de dados em vez de caminhos codificados

Por exemplo, no Windows, para armazenar os dados do perfil sob os dados do aplicativo local do usuário, em vez de no local padrão, configure a política *UserDataDir* para **${local_app_data}\Edge\Profile**.

Para saber mais, consulte [Criar variáveis de diretório de dados do usuário do Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).