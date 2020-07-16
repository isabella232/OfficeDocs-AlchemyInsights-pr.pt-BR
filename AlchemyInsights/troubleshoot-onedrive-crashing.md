---
title: Solução de problemas do OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2020
ms.locfileid: "44735383"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="a88ee-102">Solução de problemas do OneDrive</span><span class="sxs-lookup"><span data-stu-id="a88ee-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="a88ee-103">Se o OneDrive falhar repetidamente, experimente estas etapas de solução de problemas:</span><span class="sxs-lookup"><span data-stu-id="a88ee-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="a88ee-104">**Garantir que as chaves do registro não estejam definidas:**</span><span class="sxs-lookup"><span data-stu-id="a88ee-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="a88ee-105">Usando o Editor de Registro, navegue até HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="a88ee-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="a88ee-106">Se DisableFileSyncNGSC estiver presente e definido como 1, abra a chave e altere o valor para 0.</span><span class="sxs-lookup"><span data-stu-id="a88ee-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="a88ee-107">Inicie o OneDrive manualmente acessando Iniciar</span><span class="sxs-lookup"><span data-stu-id="a88ee-107">Manually launch OneDrive by going to Start</span></span> ![Pressione a tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="a88ee-109">, digite OneDrive na caixa de pesquisa e, em seguida, clique no aplicativo da área de trabalho do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a88ee-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="a88ee-110">**Redefinir o OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="a88ee-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="a88ee-111">Observações:</span><span class="sxs-lookup"><span data-stu-id="a88ee-111">Notes:</span></span>

- <span data-ttu-id="a88ee-112">Redefinir o OneDrive desconectará todas as conexões de sincronização existentes (inclusive seu OneDrive pessoal, caso esteja configurado).</span><span class="sxs-lookup"><span data-stu-id="a88ee-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="a88ee-113">Você não perde dados ou arquivos ao redefinir o OneDrive no seu computador.</span><span class="sxs-lookup"><span data-stu-id="a88ee-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="a88ee-114">**Para redefinir o OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="a88ee-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="a88ee-115">Abra uma caixa de diálogo Executar pressionando a tecla Windows e R.</span><span class="sxs-lookup"><span data-stu-id="a88ee-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="a88ee-116">Digite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset e pressione OK.</span><span class="sxs-lookup"><span data-stu-id="a88ee-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="a88ee-117">Uma janela de Comando pode aparecer durante breves instantes.</span><span class="sxs-lookup"><span data-stu-id="a88ee-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="a88ee-118">Inicie o OneDrive manualmente acessando Iniciar</span><span class="sxs-lookup"><span data-stu-id="a88ee-118">Manually launch OneDrive by going to Start</span></span> ![Pressione a tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="a88ee-120">, digite OneDrive na caixa de pesquisa e, em seguida, clique no aplicativo da área de trabalho do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a88ee-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="a88ee-121">Observações:</span><span class="sxs-lookup"><span data-stu-id="a88ee-121">Notes:</span></span>

- <span data-ttu-id="a88ee-122">Se você escolhido sincronizar apenas algumas pastas antes da redefinição, precisará fazer isso novamente após concluir a sincronização.</span><span class="sxs-lookup"><span data-stu-id="a88ee-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="a88ee-123">Leia  [Escolher quais pastas do OneDrive sincronizar com seu computador](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  para mais informações.</span><span class="sxs-lookup"><span data-stu-id="a88ee-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="a88ee-124">Será necessário concluir isso para o seu OneDrive pessoal e para o OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a88ee-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>