---
title: erro 0x8004de40 ao iniciar o OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815961"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="11c99-102">erro 0x8004de40 ao iniciar o OneDrive</span><span class="sxs-lookup"><span data-stu-id="11c99-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="11c99-103">Se você receber uma mensagem de erro **0x8004de40** ao fazer logon no onedrive, reinicie o computador enquanto estiver conectado ao seu domínio corporativo ou escolar.</span><span class="sxs-lookup"><span data-stu-id="11c99-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="11c99-104">Se você receber esse erro após a reinicialização, tente isso enquanto estiver conectado ao seu domínio corporativo ou de estudante:</span><span class="sxs-lookup"><span data-stu-id="11c99-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="11c99-105">Clique em Iniciar e digite **cmd** ou **prompt de comando**  na caixa de pesquisa, clique com o botão direito do mouse no aplicativo prompt de comando e selecione  **Executar como administrador** .</span><span class="sxs-lookup"><span data-stu-id="11c99-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="11c99-106">Se for solicitada uma senha de administrador ou uma confirmação, digite a senha ou clique em **permitir** .</span><span class="sxs-lookup"><span data-stu-id="11c99-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="11c99-107">Na janela prompt de comando, digite **dsregcmd/Leave**  e aguarde até que o comando seja concluído.</span><span class="sxs-lookup"><span data-stu-id="11c99-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="11c99-108">Em seguida, digite **dsregcmd/Join** e aguarde até que o comando seja concluído.</span><span class="sxs-lookup"><span data-stu-id="11c99-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="11c99-109">Reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="11c99-109">Reboot your computer.</span></span>
