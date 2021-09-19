---
title: Não foi possível adicionar uma conta após fazer upgrade para macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446714"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Não foi possível adicionar uma conta após fazer upgrade para macOS 11.6 Big Sur

Depois de atualizar para o macOS 11.6, sua conta do OneDrive para trabalho ou escola ou sua conta pessoal do OneDrive podem não aparecer na sua lista de contas e você pode não conseguir fazer login em uma segunda conta a partir do aplicativo.

Este é um problema emergente relacionado à atualização do macOS 11.6. Até que o problema seja resolvido, você pode acessar o conteúdo do OneDrive na web ou em seu dispositivo móvel. A Microsoft está trabalhando com a Apple para restaurar a funcionalidade do OneDrive.

Você também pode iniciar a instância do OneDrive ausente manualmente usando o Terminal. 

**Observação**: esta solução alternativa funciona apenas até que o OneDrive seja reiniciado (por uma reinicialização da máquina ou uma atualização do aplicativo OneDrive).

Se a instância ausente for a conta pessoal, abra o Terminal e digite:

`open "/Applications/OneDrive.app" --new --args /client=Personal`

Se a instância ausente for a conta de trabalho ou escola, abra o Terminal e digite:

`open "/Applications/OneDrive.app" --new --args /client=Business1`

