---
title: Níveis de permissão do SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760681"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de conexão do SharePoint Designer 

Se o SharePoint Designer estiver enfrentando problemas de conexão para sites do SharePoint, tente as seguintes soluções comuns.

Etapa 1: verificar se o SharePoint Designer foi atualizado.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Atualização para o SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Etapa 2: limpar os arquivos de cache local

- Feche o SharePoint Designer 2013.

- No computador local, navegue até as pastas a seguir para remover os arquivos armazenados em cache.

- Clique em Iniciar, executar e excluir todos os arquivos encontrados em cada um dos locais abaixo.

%APPDATA%\Microsoft\Web Server Extensions\Cache%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Abra o SharePoint Designer 2013 e insira a conta novamente para ver se ele funciona.

Etapa 3: [habilitar a autenticação moderna do Office 2013 em dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Etapa 4: os administradores precisarão permitir que o script personalizado permita a conexão com o SharePoint Designer.

Para obter etapas detalhadas, exemplos e considerações, consulte [permitir ou impedir o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


