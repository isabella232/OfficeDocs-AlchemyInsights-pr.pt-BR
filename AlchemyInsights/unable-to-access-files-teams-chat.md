---
title: Não é possível acessar arquivos compartilhados no chat do Teams
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505839"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a>Não é possível acessar arquivos compartilhados no chat do Teams

No Microsoft Teams, um arquivo compartilhado por um usuário em uma janela de chat é armazenado automaticamente no site do OneDrive do usuário de compartilhamento.

Quando outro usuário tentar abrir o arquivo no Teams e receber a mensagem de erro "Você não tem acesso a este arquivo", o problema ocorre porque o recurso do modo bloqueado de permissão do usuário de Acesso limitado é ativado no site do OneDrive.

1. Para obter instruções sobre como desabilitar o recurso no site do OneDrive, confira [Erro ao abrir um arquivo no Teams](https://go.microsoft.com/fwlink/?linkid=2155733).

1. Verifique se outro usuário tem acesso ao site do OneDrive e forneça acesso seguindo as instruções em [Compartilhar arquivos e pastas do OneDrive](https://go.microsoft.com/fwlink/?linkid=2156017).