---
title: Corrigir 0x8004de40 erro no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649736"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corrigir 0x8004de40 erro no OneDrive

Se você estiver executando o Windows 7 e receber esse erro, atualize para habilitar [o TLS 1.1 e o TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)como protocolos seguros padrão no WinHTTP no Windows .

Se você estiver executando o Windows 10 e receber um erro 0x8004de40 com o OneDrive:

- Reboot the affected computer while connected to your Acitve Directory domain.
- Se uma reinicialização não corrigir o problema, desaja e reapresente seu dispositivo do Azure AD. 

**Observação**: você deve estar em sua rede corporativa durante a execução dessas etapas. Não execute essas etapas quando você não estiver conectado à infraestrutura corporativa (por exemplo, durante a viagem). 

1. Abra um prompt de comando com privilégios elevados selecionando **Iniciar**, clique com o botão direito do mouse em Prompt de **Comando** e selecione Executar **como administrador**.

1. Digite *dsregcmd /leave e* pressione **Enter**.

1. Quando estiver concluído, digite *dsregcmd /join e* pressione **Enter**.

1. Quando estiver concluído, feche o prompt de comando.

1. Reinicie o computador e faça logoff no OneDrive.