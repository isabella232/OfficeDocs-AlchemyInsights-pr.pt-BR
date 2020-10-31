---
title: erro 0x8004de40 ao iniciar o OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815961"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>erro 0x8004de40 ao iniciar o OneDrive

Se você receber uma mensagem de erro **0x8004de40** ao fazer logon no onedrive, reinicie o computador enquanto estiver conectado ao seu domínio corporativo ou escolar. Se você receber esse erro após a reinicialização, tente isso enquanto estiver conectado ao seu domínio corporativo ou de estudante:

1. Clique em Iniciar e digite **cmd** ou **prompt de comando**  na caixa de pesquisa, clique com o botão direito do mouse no aplicativo prompt de comando e selecione  **Executar como administrador** . Se for solicitada uma senha de administrador ou uma confirmação, digite a senha ou clique em **permitir** .  

2. Na janela prompt de comando, digite **dsregcmd/Leave**  e aguarde até que o comando seja concluído. Em seguida, digite **dsregcmd/Join** e aguarde até que o comando seja concluído.
3. Reinicie o computador.
