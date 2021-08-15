---
title: Remover o serviço de plano de fundo da Pesquisa da Microsoft no Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 07d24290fc3b13cce7a931c4cff15176c080b4413489ba1935b6886939ea3874
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53982361"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Remover o serviço de plano de fundo da Pesquisa da Microsoft no Bing

Para remover o serviço de segundo plano da Pesquisa da Microsoft no Bing, experimente as seguintes medidas:

1. Para reverter para as configurações originais do mecanismo de pesquisa, faça o seguinte:

    a. Alterne o **Usar o Bing como seu mecanismo de pesquisa padrão [para](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Desligado**.

    b. [Vá para a Centro de administração do Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) e limpe a configuração que afeta todos os usuários em sua organização.

2. Para remover o serviço de segundo plano de um dispositivo individual, faça as seguintes tarefas:

    a. Vá para **Painel de controle > Programas > Programas e Recursos**.

    b. Clique com o botão direito em **Pesquisa da Microsoft no Bing** na lista de programas instalados e clique em **Desinstalar**.

3. Para remover o serviço de segundo plano de vários dispositivos da sua organização, faça logon como administrador e execute o seguinte comando em um script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
