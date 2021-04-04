---
title: Não é possível acessar arquivos compartilhados no chat do Teams
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505839"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="bd491-102">Não é possível acessar arquivos compartilhados no chat do Teams</span><span class="sxs-lookup"><span data-stu-id="bd491-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="bd491-103">No Microsoft Teams, um arquivo compartilhado por um usuário em uma janela de chat é armazenado automaticamente no site do OneDrive do usuário de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="bd491-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="bd491-104">Quando outro usuário tentar abrir o arquivo no Teams e receber a mensagem de erro "Você não tem acesso a este arquivo", o problema ocorre porque o recurso do modo bloqueado de permissão do usuário de Acesso limitado é ativado no site do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bd491-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="bd491-105">Para obter instruções sobre como desabilitar o recurso no site do OneDrive, confira [Erro ao abrir um arquivo no Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span><span class="sxs-lookup"><span data-stu-id="bd491-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="bd491-106">Verifique se outro usuário tem acesso ao site do OneDrive e forneça acesso seguindo as instruções em [Compartilhar arquivos e pastas do OneDrive](https://go.microsoft.com/fwlink/?linkid=2156017).</span><span class="sxs-lookup"><span data-stu-id="bd491-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>