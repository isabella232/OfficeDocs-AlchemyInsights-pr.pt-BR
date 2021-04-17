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
# <a name="teams-client-crashing"></a><span data-ttu-id="33105-102">Falha nos clientes do Teams?</span><span class="sxs-lookup"><span data-stu-id="33105-102">Teams client crashing?</span></span>

<span data-ttu-id="33105-103">Se o cliente de Teams estiver falhando, experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="33105-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="33105-104">Se você estiver usando o aplicativo de área de trabalho das Teams, [certifique-se de que o aplicativo esteja totalmente atualizado](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="33105-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="33105-105">Certifique-se de que todas as [URLs e intervalos de endereços do Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) estejam acessíveis.</span><span class="sxs-lookup"><span data-stu-id="33105-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="33105-106">Entre com sua conta de administrador de locatário e consulte [Painel de integridade do serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se existe erro ou degradação do serviço.</span><span class="sxs-lookup"><span data-stu-id="33105-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="33105-107">Desinstalar e reinstalar o aplicativo Teams (link)</span><span class="sxs-lookup"><span data-stu-id="33105-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="33105-108">Navegue até a pasta %appdata%\Microsoft\teams\ no computador e exclua todos os arquivos desse diretório.</span><span class="sxs-lookup"><span data-stu-id="33105-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="33105-109">[Baixar e instalar o aplicativo Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)e, se possível, instale o Teams como um administrador (clique com o botão direito do mouse no instalador Teams e selecione "Executar como administrador", se disponível).</span><span class="sxs-lookup"><span data-stu-id="33105-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="33105-110">Se o seu cliente do Teams ainda estiver travando, você pode reproduzir o problema?</span><span class="sxs-lookup"><span data-stu-id="33105-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="33105-111">Se sim:</span><span class="sxs-lookup"><span data-stu-id="33105-111">If so:</span></span>

1. <span data-ttu-id="33105-112">Use o gravador de etapas para capturar suas etapas.</span><span class="sxs-lookup"><span data-stu-id="33105-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="33105-113">Feche TODOS os aplicativos desnecessários ou confidenciais.</span><span class="sxs-lookup"><span data-stu-id="33105-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="33105-114">Inicie o Gravador de etapas e reproduza o problema enquanto estiver conectado à conta de usuário afetada.</span><span class="sxs-lookup"><span data-stu-id="33105-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="33105-115">[Reúna os logs de equipes que capturam as etapas de reprodução registradas](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="33105-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="33105-116">**Observação**: não deixe de capturar o endereço de entrada do usuário afetado.</span><span class="sxs-lookup"><span data-stu-id="33105-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="33105-117">Coletar as informações de despejo e/ou balde de falha (Windows).</span><span class="sxs-lookup"><span data-stu-id="33105-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="33105-118">Inicie o Windows PowerShell no computador onde a falha está ocorrendo e execute os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="33105-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="33105-119">Anexe o arquivo ao seu caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="33105-119">Attach the file to your support case.</span></span>
