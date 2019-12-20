---
title: Erro 4C7 do Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795944"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="ec78c-102">erro 4C7 no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ec78c-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="ec78c-103">Este erro ocorre porque o Microsoft Teams requer autenticação de formulários.</span><span class="sxs-lookup"><span data-stu-id="ec78c-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="ec78c-104">Ao implantar o AD FS (serviços de Federação do Active Directory), a autenticação de formulários não é habilitada para a intranet por padrão.</span><span class="sxs-lookup"><span data-stu-id="ec78c-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="ec78c-105">Se a autenticação integrada do Windows falhar, você será solicitado a entrar usando a autenticação de formulários.</span><span class="sxs-lookup"><span data-stu-id="ec78c-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="ec78c-106">Para resolver esse problema, habilite a autenticação de formulários usando o snap-in do MMC (console de gerenciamento Microsoft) do AD FS no computador que tem a cópia local do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ec78c-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="ec78c-107">Para fazer isso, execute estas etapas:</span><span class="sxs-lookup"><span data-stu-id="ec78c-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="ec78c-108">No painel de navegação, navegue até **políticas de autenticação**.</span><span class="sxs-lookup"><span data-stu-id="ec78c-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="ec78c-109">Em **ações** no painel de detalhes, selecione **Editar Autenticação primária global**.</span><span class="sxs-lookup"><span data-stu-id="ec78c-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="ec78c-110">Na guia **intranet** , selecione **autenticação de formulários**.</span><span class="sxs-lookup"><span data-stu-id="ec78c-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="ec78c-111">Selecione **OK** (ou **aplicar**).</span><span class="sxs-lookup"><span data-stu-id="ec78c-111">Select **OK** (or **Apply**).</span></span>