---
title: Solucionar problemas de áudio em Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 81a7f77bd6565c52ec9d752934a872e59cc11e89b90a646d17c3549d72e8a69f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039414"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Solução de problemas de áudio Windows 10

**Executar o solução de problemas de áudio**

1.  Abra as [configurações Solucionar problemas](ms-settings:troubleshoot).

2.  Selecione **Reprodução de áudio** Execute o  >  **solucionador de problemas**.

**Definir o dispositivo padrão**

Se você estiver se conectando a um dispositivo de áudio usando USB ou HDMI, talvez seja necessário definir esse dispositivo como padrão:

1. Abra **Start**  >  **Sound** e selecione **Som** ou Alterar sons **do sistema** na lista de resultados.

2.  Na guia **Reprodução,** selecione um dispositivo, selecione **Definir Padrão** e selecione **OK**.

**Verificar cabos, volume, alto-falantes e fones de ouvido**

1. Verifique se as conexões do alto-falante e do fone de ouvido estão soltas e certifique-se de que elas estão conectadas ao conector correto.

2. Verifique os níveis de energia e volume e tente aumentar todos os controles de volume.

3. Alguns alto-falantes e aplicativos têm seus próprios controles de volume; talvez seja preciso verificar todos eles para garantir que eles estão nos níveis certos.

4. Tente se conectar usando uma porta USB diferente.

**Observação**: lembre-se de que os alto-falantes podem não funcionar quando os fones de ouvido estão conectados.

**Verificar o Gerenciador de Dispositivos**

Para garantir que os drivers estão atualizados:

1. Selecione **Iniciar**, digite **Gerenciador de Dispositivos** e selecione Gerenciador de **Dispositivos** na lista de resultados.

2. Em Controladores de **som, vídeo** e jogo, selecione sua placa de som, abra-a, selecione a guia **Driver** e selecione **Atualizar Driver**.

**Observação**: Windows não encontrar um novo driver, procure um no site do fabricante do dispositivo e siga as instruções.

**Reinstalar o driver**

Se você não puder atualizar por meio do Gerenciador de Dispositivos ou encontrar um novo driver no site do fabricante, experimente estas etapas:

1. No Gerenciador de Dispositivos, clique com o botão direito do mouse (ou pressione e segure) o driver de áudio e selecione **Desinstalar**. Reinicie o dispositivo e Windows tentará reinstalar o driver.

2. Se a reinstalação do driver não funcionar, tente usar o driver de áudio genérico que vem com Windows. No Gerenciador de Dispositivos, clique com o botão direito do mouse (ou pressione e segure) seu **driver** de áudio > Software de driver de atualização Navegue pelo meu computador para obter software de driver Deixe-me escolher de uma lista de drivers de dispositivo no meu computador, selecione Dispositivo de Áudio de Alta Definição , selecione Próximo e siga as instruções para instalá-lo.  >    >    
