---
title: Corrigir problemas de Bluetooth no Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730147"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Corrigir problemas de Bluetooth no Windows 10

Se o ícone Bluetooth estiver ausente ou o Bluetooth não puder ser ativado ou desativado, convém executar a solução de problemas de Bluetooth. [Abra as configurações de solução de problemas](ms-settings:troubleshoot), clique em **Bluetooth** em **Localizar e corrigir outros problemas**, clique em **executar a solução de problemas**.

Se você não vir o ícone Bluetooth, mas o Bluetooth aparece no Gerenciador de dispositivos:

1. No Gerenciador de dispositivos, clique em **Bluetooth**. Pressione e segure (ou clique com o botão direito do mouse) o nome do adaptador Bluetooth e clique em **desinstalar dispositivo**.

2. Desligue o dispositivo do Windows, aguarde alguns segundos e ative-o novamente. O Windows tentará reinstalar o driver.

Se você instalou recentemente as atualizações do Windows 10 ou a atualização para o Windows 10, convém verificar se há atualizações de driver:

1. No Gerenciador de dispositivos, clique em **Bluetooth**e, em seguida, clique no nome do adaptador Bluetooth (que pode incluir a palavra "rádio").

2. Pressione e segure (ou clique com o botão direito do mouse) o adaptador Bluetooth e, em seguida, clique em **Atualizar**  >  **pesquisa de driver automaticamente para software de driver atualizado**. Siga as etapas e, em seguida, clique em **fechar**.

      - Se o Windows não conseguir encontrar um novo driver Bluetooth, visite o site do fabricante do computador e baixe o Driver Bluetooth mais recente de lá.

    - Depois de baixá-lo, clique em **Atualizar driver**  >  **Procurar no computador para software de driver**  >  **procure** o local onde os arquivos de driver estão armazenados > **OK**  >  **Avançar**e siga as etapas para instalar.

3. Após instalar o driver atualizado, reinicie o computador e verifique se isso corrige o problema de conexão.

Para obter mais detalhes sobre como solucionar problemas de Bluetooth, confira o artigo completo, [corrigir problemas de Bluetooth no Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).
