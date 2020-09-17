---
title: Usar a opção de desbloqueio de impressão digital no Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795232"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Usar a opção de desbloqueio de impressão digital no Windows 10

**Habilitar impressão digital do Windows Hello**

Para desbloquear o Windows 10 usando sua impressão digital, você precisa configurar a impressão digital do Windows Hello adicionando (permitindo que o Windows saiba reconhecer) pelo menos um dedo. 

1. Vá até **configurações > contas > opções de entrada** (ou clique [aqui](ms-settings:signinoptions?activationSource=GetHelp)). As opções de entrada disponíveis serão listadas. Por exemplo:

    ![Opções de entrada.](media/sign-in-options.png)

2. Clique ou toque em **impressão digital do Windows Hello**e, em seguida, clique em **Configurar**. Na janela configuração do Windows Hello, clique em **introdução**. O sensor de impressão digital será ativado e você será solicitado a colocar o dedo no sensor:

   ![Sensor de impressão digital.](media/fingerprint-sensor.png)

3. Siga as instruções que solicitarão que você examine o dedo repetidamente. Quando isso estiver concluído, você terá a opção de adicionar outros dedos que você pode querer usar para entrar. Na próxima vez que você entrar no Windows 10, você terá a opção de usar sua impressão digital para fazer isso.

**Impressão digital do Windows Hello não está disponível como uma opção de entrada**

Se a impressão digital do Windows Hello não for exibida como uma opção nas **Opções de entrada**, isso significa que o Windows não está ciente de qualquer leitor/scanner de impressão digital conectado ao seu computador ou que uma política de sistema impede seu uso (se, por exemplo, seu computador for gerenciado pelo seu local de trabalho). Para solucionar problemas: 

1. Selecione o botão **Iniciar** na barra de tarefas e procure **Gerenciador de dispositivos**.

2. Clique ou toque para abrir o **Gerenciador de dispositivos**.

3. No Gerenciador de dispositivos, expanda dispositivos biométricos clicando em sua divisa.

   ![Dispositivos biométricos.](media/biometric-devices.png)

4. O scanner de impressão digital deve ser listado como um dispositivo biométrico, como o scanner Synaptics WBDI:

   ![Dispositivos biométricos.](media/biometric-devices-expanded.png)

5. Se o scanner de impressão digital não for exibido e o scanner estiver integrado ao computador, vá para o site do fabricante do PC. Na seção suporte técnico para seu modelo de computador, procure um driver do Windows 10 para um scanner que você possa instalar.

6. Se o scanner for separado do computador (anexado via USB), vá para o site do fabricante do verificador para encontrar e instalar o software de driver de dispositivo do Windows 10 para o modelo de scanner que você tem.
