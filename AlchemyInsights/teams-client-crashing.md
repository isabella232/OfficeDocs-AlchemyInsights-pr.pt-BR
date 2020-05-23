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
ms.openlocfilehash: c49dfbf422b312f4744711d5f12b0eb83b6ebf2e
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44268760"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="18d95-102">Falha nos clientes do Teams?</span><span class="sxs-lookup"><span data-stu-id="18d95-102">Teams client crashing?</span></span>

<span data-ttu-id="18d95-103">Se o cliente de Teams estiver falhando, experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="18d95-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="18d95-104">Se você estiver usando o aplicativo de área de trabalho das Teams, [certifique-se de que o aplicativo esteja totalmente atualizado](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="18d95-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="18d95-105">Certifique-se de que todas as [URLs e intervalos de endereços do Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) estejam acessíveis.</span><span class="sxs-lookup"><span data-stu-id="18d95-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="18d95-106">Entre com sua conta de administrador de locatário e consulte [Painel de integridade do serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se existe erro ou degradação do serviço.</span><span class="sxs-lookup"><span data-stu-id="18d95-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="18d95-107">Como uma última etapa, você pode tentar limpar o cache de cliente do Teams:</span><span class="sxs-lookup"><span data-stu-id="18d95-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="18d95-108">Sair completamente do cliente do aplicativo para desktop Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="18d95-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="18d95-109">Você pode clicar com o botão direito do mouse em **Teams** na Bandeja de Ícones e clicar em **Sair**, ou executar o Gerenciador de Tarefas e eliminar completamente o processo.</span><span class="sxs-lookup"><span data-stu-id="18d95-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="18d95-110">Vá para o explorador de arquivos e digite%appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="18d95-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="18d95-111">Uma vez no diretório, você verá algumas das seguintes pastas:</span><span class="sxs-lookup"><span data-stu-id="18d95-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="18d95-112">A partir de **Cache de Aplicativos**, vá até Cache e exclua qualquer um dos arquivos no local do Cache:  %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="18d95-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="18d95-113">No **Blob_storage**, exclua todos os arquivos: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="18d95-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="18d95-114">No **Cache**, exclua todos os arquivos: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="18d95-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="18d95-115">No **banco de dados**, exclua todos os arquivos: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="18d95-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="18d95-116">No **GPUCache**, exclua todos os arquivos: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="18d95-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="18d95-117">Em **IndexedDB**, exclua o arquivo .db. db:%appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="18d95-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="18d95-118">No **Armazenamento Local**, exclua todos os arquivos: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="18d95-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="18d95-119">Por fim, no **tmp**, exclua qualquer arquivos: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="18d95-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="18d95-120">Reinicie o cliente do Teams.</span><span class="sxs-lookup"><span data-stu-id="18d95-120">Restart your Teams client.</span></span>

<span data-ttu-id="18d95-121">Se o seu cliente do Teams ainda estiver travando, você pode reproduzir o problema?</span><span class="sxs-lookup"><span data-stu-id="18d95-121">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="18d95-122">Se sim:</span><span class="sxs-lookup"><span data-stu-id="18d95-122">If so:</span></span> 

1. <span data-ttu-id="18d95-123">Use o gravador de etapas para capturar suas etapas.</span><span class="sxs-lookup"><span data-stu-id="18d95-123">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="18d95-124">Feche TODOS os aplicativos desnecessários ou confidenciais.</span><span class="sxs-lookup"><span data-stu-id="18d95-124">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="18d95-125">Inicie o Gravador de etapas e reproduza o problema enquanto estiver conectado à conta de usuário afetada.</span><span class="sxs-lookup"><span data-stu-id="18d95-125">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    
2. <span data-ttu-id="18d95-126">Anexe o arquivo ao seu caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="18d95-126">Attach the file to your support case.</span></span>
