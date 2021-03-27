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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398717"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="8234a-102">Entrar no Microsoft Edge automaticamente</span><span class="sxs-lookup"><span data-stu-id="8234a-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="8234a-103">O Microsoft Edge usa a conta padrão do sistema operacional para entrar automaticamente em um usuário de acordo com a configuração do dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="8234a-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="8234a-104">Os cenários de cada tipo de configuração de dispositivo e seu processo de entrada dependente do usuário são descritos abaixo:</span><span class="sxs-lookup"><span data-stu-id="8234a-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="8234a-105">**O dispositivo é híbrido/AAD-J**: essa opção está disponível no Windows 10, no Windows de nível inferior e nas versões de servidor correspondentes.</span><span class="sxs-lookup"><span data-stu-id="8234a-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="8234a-106">Os usuários são automaticamente assinados com suas contas do Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="8234a-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="8234a-107">**O dispositivo é ingressado** no domínio : essa opção está disponível no Windows 10, no Windows de nível inferior e nas versões de servidor correspondentes.</span><span class="sxs-lookup"><span data-stu-id="8234a-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="8234a-108">Por padrão, os usuários com contas de domínio não são automaticamente assinados; para habilitar a assinatura automática para eles, use a **política ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="8234a-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="8234a-109">Para habilitar a entrada automática para usuários com contas do Azure AD, considere a junção híbrida em seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8234a-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="8234a-110">A conta padrão do sistema operacional é uma conta **da Microsoft**: essa opção está disponível no Windows 10 RS3 (versão 1709, build 10.0.16299) e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="8234a-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="8234a-111">É improvável que o cenário ocorra em dispositivos corporativos.</span><span class="sxs-lookup"><span data-stu-id="8234a-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="8234a-112">No entanto, se a conta padrão do sistema operacional for uma conta da Microsoft, o Microsoft Edge entrará automaticamente no usuário com a conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8234a-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
