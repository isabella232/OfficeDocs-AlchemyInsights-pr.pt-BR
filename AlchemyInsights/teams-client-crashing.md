---
title: Falha nos clientes do Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030504"
---
# <a name="teams-client-crashing"></a>Falha nos clientes do Teams?

Se o cliente de Teams estiver falhando, experimente o seguinte:

- Se você estiver usando o aplicativo de área de trabalho das Teams, [certifique-se de que o aplicativo esteja totalmente atualizado](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Verifique se todas as [URLs e intervalos de endereços do Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) estão acessíveis.

- Entre com sua conta de administrador e confira o [Painel de Integridade do Serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se existe falha ou degradação do serviço.

 - Como uma última etapa, você pode tentar limpar o cache de cliente do Teams:

    1.  Sair completamente do cliente do aplicativo para desktop Microsoft Teams. Você pode clicar com o botão direito do mouse em **Teams** na Bandeja de Ícones e clicar em **Sair**, ou executar o Gerenciador de Tarefas e eliminar completamente o processo.

    2.  Vá para o explorador de arquivos e digite%appdata%\Microsoft\teams.

    3.  Uma vez no diretório, você verá algumas das seguintes pastas:

         - A partir de **Cache de Aplicativos**, vá até Cache e exclua qualquer um dos arquivos no local do Cache:  %appdata%\Microsoft\teams\application cache\cache.

        - No **Blob_storage**, exclua todos os arquivos: %appdata%\Microsoft\teams\blob_storage.

        - No **Cache**, exclua todos os arquivos: %appdata%\Microsoft\teams\Cache.

        - No **banco de dados**, exclua todos os arquivos: %appdata%\Microsoft\teams\databases.

        - No **GPUCache**, exclua todos os arquivos: %appdata%\Microsoft\teams\GPUcache.

        - Em **IndexedDB**, exclua o arquivo .db. db:%appdata%\Microsoft\teams\IndexedDB.

        - No **Armazenamento Local**, exclua todos os arquivos: %appdata%\Microsoft\teams\Local Storage.

        - Por fim, no **tmp**, exclua qualquer arquivos: %appdata%\Microsoft\teams\tmp.

    4. Reinicie o cliente do Teams.
