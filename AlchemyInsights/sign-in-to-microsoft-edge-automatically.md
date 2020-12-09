---
title: Entrar no Microsoft Edge automaticamente
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599437"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="9818f-102">Entrar no Microsoft Edge automaticamente</span><span class="sxs-lookup"><span data-stu-id="9818f-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="9818f-103">O Microsoft Edge usa a conta padrão do sistema operacional para entrar automaticamente em um usuário de acordo com a configuração do dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="9818f-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="9818f-104">Os cenários de cada tipo de configuração de dispositivo e seu processo de entrada dependente de usuário são descritos abaixo:</span><span class="sxs-lookup"><span data-stu-id="9818f-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="9818f-105">**O dispositivo é híbrido/AAD-J**: essa opção está disponível no Windows 10, no Windows de nível inferior e nas versões de servidor correspondentes.</span><span class="sxs-lookup"><span data-stu-id="9818f-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="9818f-106">Os usuários são conectados automaticamente às suas contas do Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="9818f-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="9818f-107">**O dispositivo está associado ao domínio**: essa opção está disponível no Windows 10, no Windows de nível inferior e nas versões de servidor correspondentes.</span><span class="sxs-lookup"><span data-stu-id="9818f-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="9818f-108">Por padrão, os usuários com contas de domínio não são conectados automaticamente; para habilitar a entrada automática, use a política **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="9818f-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="9818f-109">Para habilitar a entrada automática para usuários com contas do Azure AD, considere o ingresso híbrido de seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9818f-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="9818f-110">**A conta padrão do sistema operacional é uma conta da Microsoft**: essa opção está disponível no Windows 10 RS3 (versão 1709, Build 10.0.16299) e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="9818f-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="9818f-111">O cenário provavelmente ocorrerá em dispositivos corporativos.</span><span class="sxs-lookup"><span data-stu-id="9818f-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="9818f-112">No entanto, se a conta padrão do sistema operacional for uma conta da Microsoft, o Microsoft Edge entrará automaticamente no usuário com a conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9818f-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
