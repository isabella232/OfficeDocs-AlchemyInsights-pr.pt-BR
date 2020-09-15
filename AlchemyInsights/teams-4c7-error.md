---
title: Erro 4c7 do Teams
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700191"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="7c2c4-102">Erro 4c7 no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7c2c4-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="7c2c4-103">Este erro ocorre porque o Microsoft Teams requer autenticação de formulários.</span><span class="sxs-lookup"><span data-stu-id="7c2c4-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="7c2c4-104">Ao implantar o Serviços de Federação do Active Directory (AD FS), a Autenticação de Formulários não é habilitada para a intranet por padrão.</span><span class="sxs-lookup"><span data-stu-id="7c2c4-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="7c2c4-105">Se a Autenticação Integrada do Windows falhar, você será solicitado a entrar usando Autenticação de Formulários.</span><span class="sxs-lookup"><span data-stu-id="7c2c4-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="7c2c4-106">Para resolver esse problema, habilite a Autenticação de Formulários usando o snap-in do MMC (Console de Gerenciamento Microsoft) do Serviços de Federação do Active Directory (AD FS) no computador que tem a cópia local do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7c2c4-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="7c2c4-107">Para fazer isso, execute estas etapas:</span><span class="sxs-lookup"><span data-stu-id="7c2c4-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="7c2c4-108">No painel de navegação, navegue até **Políticas de Autenticação**.</span><span class="sxs-lookup"><span data-stu-id="7c2c4-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="7c2c4-109">Em **Ações**, no painel detalhes, selecione **Edite a Autenticação Primária Global**.</span><span class="sxs-lookup"><span data-stu-id="7c2c4-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="7c2c4-110">Na guia **Intranet**, selecione **Autenticação de Formulários**.</span><span class="sxs-lookup"><span data-stu-id="7c2c4-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="7c2c4-111">Selecione **OK** (ou **Salvar**). </span><span class="sxs-lookup"><span data-stu-id="7c2c4-111">Select **OK** (or **Apply**).</span></span>