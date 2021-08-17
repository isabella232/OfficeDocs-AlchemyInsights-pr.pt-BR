---
title: Ocorreu um erro nos clientes do Teams?
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890326"
---
# <a name="teams-client-crashing"></a>Ocorreu um erro nos clientes do Teams?

Se o cliente de Teams estiver falhando, experimente o seguinte:

- Se você estiver usando o aplicativo de área de trabalho das Teams, [certifique-se de que o aplicativo esteja totalmente atualizado](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Certifique-se de que todas as [URLs e intervalos de endereços do Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) estejam acessíveis.

- Entre com sua conta de administrador de locatário e consulte [Painel de integridade do serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se existe erro ou degradação do serviço.

- Desinstalar e reinstalar o aplicativo Teams
    - Navegue até a pasta %appdata%\Microsoft\teams\ no seu computador e exclua todos os arquivos desse diretório.
    - [Baixe e instale o aplicativo Teams](https://www.microsoft.com/microsoft-teams/download-app)e, se possível, instale o Teams como administrador (clique com o botão direito do mouse no instalador do Teams e selecione **Executar como administrador**, se disponível).

Se o seu cliente do Teams ainda estiver travando, tente reproduzir o problema. Se você puder:

1. Use o gravador de etapas para capturar suas etapas.
    - Feche TODOS os aplicativos desnecessários ou confidenciais.
    - Inicie o Gravador de etapas e reproduza o problema enquanto estiver conectado à conta de usuário afetada.
    - [Reúna os logs de equipes que capturam as etapas de reprodução registradas](https://docs.microsoft.com/microsoftteams/log-files). **Observação**: não deixe de capturar o endereço de entrada do usuário afetado.
    - Coletar as informações de despejo e/ou bucket de falha (Windows).Inicie o Windows PowerShell no computador onde o erro está ocorrendo e execute os seguintes comandos (depois de cada comando, pressione Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Depois que o arquivo de texto for gerado e exibido na sua tela, salve o arquivo e anexe-o à solicitação de serviço. 
