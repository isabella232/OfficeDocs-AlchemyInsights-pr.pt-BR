---
title: Corrigir o erro 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052025"
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