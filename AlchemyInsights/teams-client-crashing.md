---
title: Falha nos clientes do Teams?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826259"
---
# <a name="teams-client-crashing"></a>Falha nos clientes do Teams?

Se o cliente de Teams estiver falhando, experimente o seguinte:

- Se você estiver usando o aplicativo de área de trabalho das Teams, [certifique-se de que o aplicativo esteja totalmente atualizado](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Certifique-se de que todas as [URLs e intervalos de endereços do Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) estejam acessíveis.

- Entre com sua conta de administrador de locatário e consulte [Painel de integridade do serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se existe erro ou degradação do serviço.

- Desinstalar e reinstalar o aplicativo Teams (link)
    - Navegue até a pasta %appdata%\Microsoft\teams\ no computador e exclua todos os arquivos desse diretório.
    - [Baixar e instalar o aplicativo Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)e, se possível, instale o Teams como um administrador (clique com o botão direito do mouse no instalador Teams e selecione "Executar como administrador", se disponível).

Se o seu cliente do Teams ainda estiver travando, você pode reproduzir o problema? Se sim:

1. Use o gravador de etapas para capturar suas etapas.
    - Feche TODOS os aplicativos desnecessários ou confidenciais.
    - Inicie o Gravador de etapas e reproduza o problema enquanto estiver conectado à conta de usuário afetada.
    - [Reúna os logs de equipes que capturam as etapas de reprodução registradas](https://docs.microsoft.com/microsoftteams/log-files). **Observação**: não deixe de capturar o endereço de entrada do usuário afetado.
    - Coletar as informações de despejo e/ou balde de falha (Windows). Inicie o Windows PowerShell no computador onde a falha está ocorrendo e execute os seguintes comandos:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Anexe o arquivo ao seu caso de suporte.
