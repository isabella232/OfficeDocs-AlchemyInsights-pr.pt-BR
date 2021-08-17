---
title: 'Erro: não podemos carregar ou baixar suas alterações porque suas credenciais armazenadas em cache expiraram'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 623c2f1175ed2ab9638e742521395fe62ba9cad9d21b517f17426fb5c96a2d73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059430"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a>Erro: não podemos carregar ou baixar suas alterações porque suas credenciais armazenadas em cache expiraram

Ao salvar arquivos no aplicativo OneDrive, se você receber um erro que contenha a frase **"suas credenciais armazenadas** em cache expiraram" , execute as seguintes etapas:

1. Feche todos os aplicativos do Office.
1. Abra o Gerenciador de Credenciais e digite **o gerenciador de** credenciais na caixa de pesquisa na barra de tarefas e selecione Painel de Controle do Gerenciador de **Credenciais.**
1. Selecione **Windows Credenciais**.
1. Encontre qualquer entrada que comece com a palavra **OneDrive**.
1. Selecione a entrada e pressione **Remover**.
1. Feche o Gerenciador de Credenciais, clique com o botão direito do mouse na nuvem azul em seu systray e selecione **Fechar OneDrive**.
1. Digite **OneDrive** na caixa de pesquisa na barra de tarefas e selecione **OneDrive App** para iniciar OneDrive.
1. Entre OneDrive e tente salvar o arquivo para OneDrive.
