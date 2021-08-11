---
title: Configurações de inicialização em Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909814"
---
# <a name="startup-settings-in-windows-10"></a>Configurações de inicialização em Windows 10

**Alterar quais aplicativos são executados automaticamente na inicialização**

1. Vá para [Configurações > Aplicativos > Inicialização](ms-settings:startupapps?activationSource=GetHelp).

2. Certifique-se de que qualquer aplicativo que você deseja executar na inicialização está **ligado**.

**Adicionar um aplicativo para ser executado automaticamente na inicialização**

1. Clique ou toque **em Iniciar** e encontre o aplicativo que você deseja executar na inicialização.

2. Clique com o botão direito do mouse no aplicativo, clique em **Mais** e clique **em Abrir local do arquivo**. Isso abre o local onde o atalho para o aplicativo é salvo. Se não houver opção para o local do arquivo Open, isso significa que o aplicativo não pode ser executado na inicialização.

3. Com o local do arquivo aberto, pressione a tecla **de logo Windows + R**, digite **shell:inicialização** e clique em **OK**. Isso abre a pasta Inicialização.

4. Copie e colar o atalho para o aplicativo do local do arquivo para a pasta Inicialização.

**Opções de inicialização avançadas (incluindo Cofre, configurações uefi e inicialização de outro dispositivo)**

1. Salve seu trabalho e feche todos os documentos abertos, pois essas etapas reiniciarão o computador.

2. Vá para [Configurações > Atualizar & Segurança > Recuperação](ms-settings:recovery?activationSource=GetHelp).

3. Em **Inicialização avançada,** clique **em Reiniciar agora**. 

4. Depois que o computador é reiniciado para a tela Escolher uma opção:

    - Para inicializar de um dispositivo como uma unidade USB, clique **em Usar um dispositivo**.

    - Para inserir as configurações uefi (às vezes chamada de configuração do BIOS), clique em Solucionar problemas > opções avançadas > **firmware uefi Configurações**. 

    - Para inserir Cofre modo ou alterar configurações de inicialização avançadas, clique em Solucionar problemas > opções avançadas > **inicialização Configurações,** em seguida, clique em **Reiniciar**. Você pode ser solicitado a inserir sua chave de [recuperação do BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Depois que o computador reiniciar novamente, clique na configuração de inicialização que você deseja usar.