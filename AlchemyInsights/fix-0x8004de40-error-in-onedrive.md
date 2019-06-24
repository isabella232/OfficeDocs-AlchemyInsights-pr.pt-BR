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
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133965"
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