---
title: Corrigir o erro 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716016"
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