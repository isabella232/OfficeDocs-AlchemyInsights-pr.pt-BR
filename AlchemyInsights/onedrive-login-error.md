---
title: Erro de logon do OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947471"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="91304-102">Erro de logon do OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="91304-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="91304-103">Se você receber uma mensagem de erro "AADSTS50011: a URL de resposta especificada na solicitação não corresponde à resposta" ao entrar no aplicativo OneDrive, verifique o seguinte:</span><span class="sxs-lookup"><span data-stu-id="91304-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="91304-104">Sua versão do OneDrive precisa ser igual ou superior à versão 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="91304-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="91304-105">Para verificar sua versão, clique no ícone azul do OneDrive na área de notificação, selecione **ajuda & configurações > configurações > sobre**.</span><span class="sxs-lookup"><span data-stu-id="91304-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="91304-106">Sua rede pode bloquear o tráfego para o **g.Live.com** e o **oneclient.SFX.ms**.</span><span class="sxs-lookup"><span data-stu-id="91304-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="91304-107">Se esse tráfego estiver bloqueado, o OneDrive não poderá se atualizar.</span><span class="sxs-lookup"><span data-stu-id="91304-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="91304-108">Trabalhe com seu administrador de rede para garantir que você tenha acesso a essas URLs.</span><span class="sxs-lookup"><span data-stu-id="91304-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="91304-109">[Esses pontos de extremidade](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) devem ser acessíveis para clientes que usam o Microsoft 365 Plans.</span><span class="sxs-lookup"><span data-stu-id="91304-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="91304-110">Se você precisar obter uma versão atual do OneDrive, acesse [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="91304-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
