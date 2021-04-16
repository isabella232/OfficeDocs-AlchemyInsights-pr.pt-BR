---
title: 0x8004de40 erro ao iniciar o OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813640"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 erro ao iniciar o OneDrive

Se você receber um erro **0x8004de40** ao entrar no OneDrive, reinicie o computador enquanto estiver conectado ao seu domínio de trabalho ou de estudante. Se você receber esse erro após a reinicialização, experimente isso enquanto estiver conectado ao seu domínio de trabalho ou escola:

1. Clique em Iniciar e digite **cmd** ou **prompt**  de comando na caixa de pesquisa, clique com o botão direito do mouse no aplicativo de prompt de comando e selecione  **Executar como administrador**. Se você for solicitado a solicitar uma senha de administrador ou para uma confirmação, digite a senha ou clique em **Permitir**.  

2. Na janela Prompt de Comando, digite **dsregcmd /leave**  e aguarde a conclusão do comando. Em seguida, **digite dsregcmd /join** e aguarde a conclusão do comando.
3. Reinicie o computador.
