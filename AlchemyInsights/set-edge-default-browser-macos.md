---
title: Definir o Microsoft Edge como navegador padrão em um dispositivo macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426757"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Definir o Microsoft Edge como navegador padrão em um dispositivo macOS

Use um desses dois métodos para definir o Microsoft Edge como navegador padrão:

Método 1: Atualize o dispositivo com uma imagem do macOS onde o Microsoft Edge já foi configurado como navegador padrão.

Método 2: Defina a política DefaultBrowserSettingEnabled para solicitar ao usuário que defina o Microsoft Edge como navegador padrão.

Qualquer um dos métodos permite que o usuário altere o navegador padrão. Por esse motivo, recomendamos que você implante a política DefaultBrowserSettingEnabled mesmo se tiver usado o método 1. Se um usuário alterar o navegador padrão depois que a política for implantada, a política solicitará que o usuário defina o navegador padrão de volta para o Microsoft Edge.
