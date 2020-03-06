---
title: Configurações de inicialização no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2020
ms.locfileid: "42408907"
---
# <a name="startup-settings-in-windows-10"></a>Configurações de inicialização no Windows 10

**Alterar quais aplicativos são executados automaticamente na inicialização**

1. Vá até [configurações > aplicativos > inicialização](ms-settings:startupapps?activationSource=GetHelp).

2. Certifique-se **de**que qualquer aplicativo que você deseja executar na inicialização esteja ativado.

**Adicionar um aplicativo para ser executado automaticamente na inicialização**

1. Clique ou toque em **Iniciar** e localize o aplicativo que você deseja executar na inicialização.

2. Clique com o botão direito do mouse no aplicativo, clique em **mais**e, em seguida, clique em **abrir local do arquivo**. Isso abre o local onde o atalho para o aplicativo é salvo. Se não houver opção para abrir o local do arquivo, isso significa que o aplicativo não pode ser executado na inicialização.

3. Com o local do arquivo aberto, pressione a **tecla do logotipo do Windows + R**, digite **shell: Startup**e clique em **OK**. Isso abre a pasta inicialização.

4. Copie e cole o atalho para o aplicativo do local do arquivo para a pasta de inicialização.

**Opções avançadas de inicialização (incluindo o modo de segurança, configurações de UEFI e inicialização a partir de outro dispositivo)**

1. Salve seu trabalho e feche todos os documentos abertos, pois essas etapas reiniciarão seu computador.

2. Vá até [configurações > atualização & segurança > recuperação](ms-settings:recovery?activationSource=GetHelp).

3. Em **inicialização avançada**, clique em **reiniciar agora**. 

4. Após a reinicialização do computador para a tela escolha uma opção:

    - Para inicializar a partir de um dispositivo como uma unidade USB, clique em **usar um dispositivo**.

    - Para inserir as configurações de UEFI (às vezes chamadas de configuração de BIOS), clique em **solucionar problemas > opções avançadas > configurações de firmware UEFI**. 

    - Para inserir o modo de segurança ou alterar as configurações de inicialização avançadas, clique em **solucionar problemas > opções avançadas > configurações de inicialização**e clique em **reiniciar**. Você pode ser solicitado a inserir sua [chave de recuperação do BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Após reiniciar o computador, clique na configuração de inicialização que você deseja usar.