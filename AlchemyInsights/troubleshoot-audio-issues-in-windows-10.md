---
title: Solucionar problemas de áudio no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795947"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a>Solucionando problemas de áudio no Windows 10

**Executar a solução de problemas de áudio**

A solução de problemas de áudio pode ser capaz de corrigir os problemas de áudio automaticamente: 

1. Selecione **Iniciar**, digite **solução de problemas**e selecione **solucionar problemas** na lista de resultados. 
2. Selecione **reproduzindo áudio** > **Execute a solução de problemas**.

**Verificar cabos, volume, alto-falantes e fones de ouvido**

- Verifique se há cabos soltos nas conexões do alto-falante e do fone de ouvido e certifique-se de que estão conectados ao conector correto.
- Verifique os níveis de energia e de volume e tente ativar todos os controles de volume.
- Alguns alto-falantes e aplicativos têm seus próprios controles de volume e você pode precisar verificá-los para garantir que estejam nos níveis corretos.
- Tente se conectar usando uma porta USB diferente.
- **Observação:** Lembre-se de que os alto-falantes podem não funcionar quando os fones de ouvido estiverem conectados.

**Verificar o Gerenciador de dispositivos**

Para certificar-se de que os drivers estão atualizados:

- Selecione **Iniciar**, digite **Gerenciador de dispositivos**e, em seguida, selecione **Gerenciador de dispositivos** na lista de resultados.

2. Em **controladores de som, vídeo e jogo**, selecione sua placa de som, abra-a, selecione a guia **Driver** e selecione **Atualizar driver**. 

**Observação:** Se o Windows não encontrar um novo driver, procure um no site do fabricante do dispositivo e siga as instruções.

**Reinstalar o driver**

Se você não conseguir atualizar por meio do Gerenciador de dispositivos ou encontrar um novo driver no site do fabricante, tente estas etapas: 

1. No Gerenciador de dispositivos, clique com o botão direito do mouse (ou pressione e segure) no driver de áudio e selecione **desinstalar**. Reinicie o dispositivo e o Windows tentará reinstalar o driver.

2. Se a reinstalação do driver não funcionar, tente usar o driver de áudio genérico fornecido com o Windows. No Gerenciador de dispositivos, clique com o botão direito do mouse (ou pressione e segure) seu driver de áudio > **Atualizar driver software** > **procurar meu computador para software** > de driver**deixe-me escolher em uma lista de drivers de dispositivo no meu computador**, selecione **dispositivo de áudio de alta definição**, selecione **Avançar**e siga as instruções para instalá-lo.

**Definir o dispositivo padrão**

Se você estiver se conectando a um dispositivo de áudio usando USB ou HDMI, talvez precise definir esse dispositivo como o padrão: 

1. Selecione **Iniciar**, digite **som**e, em seguida, selecione **som** ou **alterar sons do sistema** na lista de resultados.

2. Na guia **reprodução** , selecione um dispositivo, selecione **definir padrão**e, em seguida, selecione **OK**.

