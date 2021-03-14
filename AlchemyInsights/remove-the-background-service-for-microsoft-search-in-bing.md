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
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753378"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Remover o serviço de plano de fundo da Pesquisa da Microsoft no Bing

Para remover o serviço de segundo plano da Pesquisa da Microsoft no Bing, experimente as seguintes medidas:

1. Para reverter para as configurações originais do mecanismo de pesquisa, faça o seguinte:

    a. Alterne o **Use o Bing como seu mecanismo de pesquisa padrão [para](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Desligado**.

    b. [Vá para a Centro de administração do Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) e limpe a configuração que afeta todos os usuários em sua organização.

2. Para remover o serviço de segundo plano de um dispositivo individual, faça as seguintes tarefas:

    a. Vá para **Painel de controle > Programas > Programas e Recursos**.

    b. Clique com o botão direito em **Pesquisa da Microsoft no Bing** na lista de programas instalados e clique em **Desinstalar**.

3. Para remover o serviço de segundo plano de vários dispositivos da sua organização, faça logon como administrador e execute o seguinte comando em um script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
