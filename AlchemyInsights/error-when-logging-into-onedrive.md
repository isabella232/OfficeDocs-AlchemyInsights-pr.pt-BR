---
title: 0x8004de40 erro ao iniciar OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946567"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 erro ao iniciar OneDrive

Se você receber um erro **0x8004de40** ao entrar no OneDrive, reinicie o computador enquanto estiver conectado ao seu domínio de trabalho ou escola. Se você receber esse erro após a reinicialização, experimente isso enquanto estiver conectado ao seu domínio de trabalho ou escola:

1. Clique em Iniciar e digite **cmd** ou **prompt**  de comando na caixa de pesquisa, clique com o botão direito do mouse no aplicativo de prompt de comando e selecione  **Executar como administrador**. Se você for solicitado a solicitar uma senha de administrador ou para uma confirmação, digite a senha ou clique em **Permitir**.  

2. Na janela Prompt de Comando, digite **dsregcmd /leave**  e aguarde a conclusão do comando. Em seguida, **digite dsregcmd /join** e aguarde a conclusão do comando.
3. Reinicie o computador.
