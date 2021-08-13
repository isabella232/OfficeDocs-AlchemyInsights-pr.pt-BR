---
title: Liberar espaço em disco no Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928069"
---
# <a name="free-up-drive-space-in-windows-10"></a>Liberar espaço em disco no Windows 10

Veja duas opções para liberar espaço em disco no Windows:

- Libere espaço em disco no Windows 10.
- Libere espaço para atualizações do Windows 10 com um dispositivo de armazenamento externo.

Se você ainda tiver pouco espaço em disco após usar a Limpeza de Disco, é possível que sua pasta Temp esteja enchendo rapidamente com arquivos de aplicativos (.appx) usados pela Microsoft Store. Para resolver esse problema, redefina a Store, limpe o cache dela e, em seguida, execute a solução de problemas do Windows Update. Verifique se a Microsoft Store está fechada antes de prosseguir com estas etapas.

**Etapa 1: Redefinir a Microsoft Store**

**Observação** Isso exclui permanentemente os dados do aplicativo no dispositivo, incluindo suas preferências e detalhes de entrada.

1. Selecione **Iniciar** > **Configurações** > **Aplicativos** > **Aplicativos e recursos**.

1. Na lista de aplicativos, localize e selecione a Microsoft Store.

1. Selecione **Opções avançadas**.

1. Role para baixo, selecione **Redefinir** e, em seguida **Confirmar Redefinição**.

**Etapa 2: Limpar o cache da Microsoft Store**

1. Pressione a Tecla do Logotipo do Windows + R para abrir a caixa de diálogo Executar.

1. Digite wsreset.exe e selecione **OK**.

1. Uma janela vazia do Prompt de Comando será aberta. Após cerca de 10 segundos, a janela se fecha e a Store será aberta automaticamente.

**Etapa 3: Redefinir o Windows Update**

1. Selecione **Iniciar** > **Configurações** > **Atualização e Segurança** > **Solucionar problemas**.

1. Role para baixo, selecione **Windows Update** na lista e, em seguida, **Executar a solução de problemas**.

1. Reinicie o computador e verifique se você continua tendo problemas.

