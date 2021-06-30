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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187709"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="9a231-102">Ocorreu um erro nos clientes do Teams?</span><span class="sxs-lookup"><span data-stu-id="9a231-102">Teams client crashing</span></span>

<span data-ttu-id="9a231-103">Se o cliente de Teams estiver falhando, experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9a231-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="9a231-104">Se você estiver usando o aplicativo de área de trabalho das Teams, [certifique-se de que o aplicativo esteja totalmente atualizado](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="9a231-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="9a231-105">Certifique-se de que todas as [URLs e intervalos de endereços do Office 365](/microsoftteams/connectivity-issues) estejam acessíveis.</span><span class="sxs-lookup"><span data-stu-id="9a231-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="9a231-106">Entre com sua conta de administrador de locatário e consulte [Painel de integridade do serviço](/office365/enterprise/view-service-health) para verificar se existe erro ou degradação do serviço.</span><span class="sxs-lookup"><span data-stu-id="9a231-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="9a231-107">Desinstalar e reinstalar o aplicativo Teams</span><span class="sxs-lookup"><span data-stu-id="9a231-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="9a231-108">Navegue até a pasta %appdata%\Microsoft\teams\ no seu computador e exclua todos os arquivos desse diretório.</span><span class="sxs-lookup"><span data-stu-id="9a231-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="9a231-109">[Baixe e instale o aplicativo Teams](https://www.microsoft.com/microsoft-teams/download-app)e, se possível, instale o Teams como administrador (clique com o botão direito do mouse no instalador do Teams e selecione **Executar como administrador**, se disponível).</span><span class="sxs-lookup"><span data-stu-id="9a231-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="9a231-110">Se o seu cliente do Teams ainda estiver travando, tente reproduzir o problema.</span><span class="sxs-lookup"><span data-stu-id="9a231-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="9a231-111">Se você puder:</span><span class="sxs-lookup"><span data-stu-id="9a231-111">If you can:</span></span>

1. <span data-ttu-id="9a231-112">Use o gravador de etapas para capturar suas etapas.</span><span class="sxs-lookup"><span data-stu-id="9a231-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="9a231-113">Feche TODOS os aplicativos desnecessários ou confidenciais.</span><span class="sxs-lookup"><span data-stu-id="9a231-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="9a231-114">Inicie o Gravador de etapas e reproduza o problema enquanto estiver conectado à conta de usuário afetada.</span><span class="sxs-lookup"><span data-stu-id="9a231-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="9a231-115">[Reúna os logs de equipes que capturam as etapas de reprodução registradas](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="9a231-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="9a231-116">**Observação**: não deixe de capturar o endereço de entrada do usuário afetado.</span><span class="sxs-lookup"><span data-stu-id="9a231-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="9a231-117">Coletar as informações de despejo e/ou balde de falha (Windows).</span><span class="sxs-lookup"><span data-stu-id="9a231-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="9a231-118">Inicie o Windows PowerShell no computador onde o erro está ocorrendo e execute os seguintes comandos (depois de cada comando, pressione Enter):</span><span class="sxs-lookup"><span data-stu-id="9a231-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="9a231-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="9a231-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="9a231-120">Depois que o arquivo de texto for gerado e exibido na sua tela, salve o arquivo e anexe-o à solicitação de serviço.</span><span class="sxs-lookup"><span data-stu-id="9a231-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
