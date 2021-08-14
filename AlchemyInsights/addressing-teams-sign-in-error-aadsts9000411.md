---
title: Abordando o erro AADSTS9000411 de entrada no Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952996"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Abordando o erro AADSTS9000411 de entrada no Teams

Ao entrar no Microsoft Teams, você pode receber a mensagem de erro: **Infelizmente, estamos com problemas para entrar AADSTS9000411: a solicitação não foi formatada corretamente. O parâmetro "login_hint" está duplicado.**

Para resolver esse problema, certifique-se de que os clientes do Microsoft Teams estejam atualizados. Para obter mais informações sobre como atualizar seu cliente, confira [Atualizar o Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Se você não puder atualizar o seu cliente por algum motivo, a desconexão do cliente limpará a maioria dos dados armazenados em cache. No entanto, se você continuar enfrentando dificuldades sair/entrar, apague o Teams e limpe o cache do cliente fazendo o seguinte:
1. Feche o Microsoft Teams.
2. Vá para: %appdata%\microsoft\teams e delete todos os arquivos.
3. Reabra o Microsoft Teams.
