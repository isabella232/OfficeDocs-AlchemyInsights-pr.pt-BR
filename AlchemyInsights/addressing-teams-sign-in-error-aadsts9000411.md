---
title: Abordando o erro AADSTS9000411 de entrada no Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44328778"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="9d0dc-102">Abordando o erro AADSTS9000411 de entrada no Teams</span><span class="sxs-lookup"><span data-stu-id="9d0dc-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="9d0dc-103">Ao entrar no Microsoft Teams, você pode receber a mensagem de erro: **Infelizmente, estamos com problemas para entrar AADSTS9000411: a solicitação não foi formatada corretamente. O parâmetro "login_hint" está duplicado.**</span><span class="sxs-lookup"><span data-stu-id="9d0dc-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="9d0dc-104">Para resolver esse problema, certifique-se de que os clientes do Microsoft Teams estejam atualizados.</span><span class="sxs-lookup"><span data-stu-id="9d0dc-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="9d0dc-105">Para obter mais informações sobre como atualizar seu cliente, confira [Atualizar o Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="9d0dc-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="9d0dc-106">Se você não puder atualizar o seu cliente por algum motivo, a desconexão do cliente limpará a maioria dos dados armazenados em cache.</span><span class="sxs-lookup"><span data-stu-id="9d0dc-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="9d0dc-107">No entanto, se você continuar enfrentando dificuldades sair/entrar, apague o Teams e limpe o cache do cliente fazendo o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9d0dc-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="9d0dc-108">Feche o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9d0dc-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="9d0dc-109">Vá para: %appdata%\microsoft\teams e delete todos os arquivos.</span><span class="sxs-lookup"><span data-stu-id="9d0dc-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="9d0dc-110">Reabra o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9d0dc-110">Reopen Microsoft Teams.</span></span>
