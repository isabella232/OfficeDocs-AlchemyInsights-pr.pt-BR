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
ms.openlocfilehash: 42731693c062b961bdd3bf7b728ea64f705765e539ee751903dd57f263d11ae0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54092408"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a>Não é possível acessar arquivos compartilhados no chat do Teams

No Microsoft Teams, um arquivo compartilhado por um usuário em uma janela de chat é armazenado automaticamente no site do OneDrive do usuário de compartilhamento.

Quando outro usuário tentar abrir o arquivo no Teams e receber a mensagem de erro "Você não tem acesso a este arquivo", o problema ocorre porque o recurso do modo bloqueado de permissão do usuário de Acesso limitado é ativado no site do OneDrive.

1. Para obter instruções sobre como desabilitar o recurso no site do OneDrive, confira [Erro ao abrir um arquivo no Teams](https://go.microsoft.com/fwlink/?linkid=2155733).

1. Verifique se outro usuário tem acesso ao site do OneDrive e forneça acesso seguindo as instruções em [Compartilhar arquivos e pastas do OneDrive](https://go.microsoft.com/fwlink/?linkid=2156017).