---
title: Corrigir o erro 0x8004de40 no OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525047"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corrigir o erro 0x8004de40 no OneDrive

Se você receber um erro 0x8004de40 com o OneDrive:

- Reinicie o computador afetado enquanto estiver conectado ao seu domínio de diretório do acitve.
- Se uma reinicialização não corrigir o problema, desingresse e reingresse seu dispositivo do Azure AD. 

**Observação**: você deve estar em sua rede corporativa enquanto executa estas etapas. Não execute estas etapas quando não puder se conectar à infraestrutura corporativa (por exemplo, ao viajar). 

- Abra um prompt de comando com privilégios elevados. 
- Para abrir um prompt de comando com privilégios elevados, clique em **Iniciar**, clique com o botão direito do mouse em **prompt de comando**e clique em **Executar como administrador**.
- Digite *dsregcmd/Leave* e pressione **Enter**.
- Ao concluir, digite *dsregcmd/Join* e pressione **Enter**.
- Ao concluir, feche o prompt de comando.
- Reinicie o computador e faça logon no OneDrive.