---
title: Problemas de conexão do SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508411"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de conexão do SharePoint Designer 

Se o SharePoint Designer estiver enfrentando problemas de conexão para sites do SharePoint, tente as soluções comuns a seguir.

Etapa 1: verificar se o SharePoint Designer 2013 foi atualizado com o [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e a [atualização de 2 de agosto de 2016 para o SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Etapa 2: limpar os arquivos de cache local:

1. Feche o SharePoint Designer 2013.

2. No computador local, remova todos os arquivos encontrados em cada uma das pastas a seguir.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Abra o SharePoint Designer 2013 e insira a conta novamente para ver se ele funciona.

Etapa 3: [habilitar a autenticação moderna do Office 2013 em dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Etapa 4: os administradores precisarão **permitir o script personalizado** nas configurações do centro de administração do SharePoint para permitir a conexão com o SharePoint Designer. Consulte [permitir ou impedir o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obter mais informações.


