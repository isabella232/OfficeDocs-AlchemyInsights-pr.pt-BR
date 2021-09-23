---
title: Não foi possível adicionar uma conta após fazer upgrade para macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475123"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Não foi possível adicionar uma conta após fazer upgrade para macOS 11.6 Big Sur

Depois de atualizar para o macOS 11.6, sua conta do OneDrive para trabalho ou escola ou sua conta pessoal do OneDrive podem não aparecer na sua lista de contas e você pode não conseguir fazer login em uma segunda conta a partir do aplicativo.

Uma correção foi desenvolvida para esse problema. Primeiro, determine se você está executando a versão autônoma ou App Store do OneDrive:

- Selecione a nuvem do OneDrive na barra de menus > **Ajuda e Configurações** > **Preferências** > **Sobre**. Se o número da versão não incluir **(Autônomo)**, você terá a versão do produto da App Store.

Se você estiver usando a versão autônoma do OneDrive, reinicie o computador e as atualizações automáticas do OneDrive para um build em que esse problema seja resolvido. Se você quiser instalar o build manualmente, baixe este [arquivo zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip), descompacte o arquivo e copie o aplicativo OneDrive para a pasta Aplicativos (substituindo o aplicativo existente do OneDrive).

Se você estiver usando a versão da App Store, considere instalar a versão autônoma do OneDrive. Esta versão funciona da mesma maneira que a versão da App Store, mas permite que a Microsoft ofereça atualizações mais rapidamente aos usuários e as conecta a uma versão que inclui a correção para esse problema.

1. Baixe a versão autônoma do [OneDrive que inclui a correção](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip).
2. Descompacte o arquivo e copie o aplicativo OneDrive para a pasta Aplicativos (substituindo o aplicativo existente do OneDrive).

Se você precisar usar a versão da App Store, aguarde até que a App Store lance uma versão do aplicativo que inclua a correção. Infelizmente, a Microsoft não pode comunicar uma data estimada para que uma versão fixa seja lançada na App Store.


