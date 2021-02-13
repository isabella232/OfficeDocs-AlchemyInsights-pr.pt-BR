---
title: Implantar o Microsoft Edge para iOS, iPadOS e Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177985"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="129fd-102">Implantar o Microsoft Edge para iOS, iPadOS e Android</span><span class="sxs-lookup"><span data-stu-id="129fd-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="129fd-103">O cenário guiado resumido abaixo o ajudará a atribuir o Microsoft Edge a usuários de dispositivos iOS, iPadOS e Android.</span><span class="sxs-lookup"><span data-stu-id="129fd-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="129fd-104">Se você bloqueou o registro de dispositivos móveis pelos usuários, este cenário guiado não funcionará e os usuários precisarão instalar o Microsoft Edge por conta própria.</span><span class="sxs-lookup"><span data-stu-id="129fd-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="129fd-105">O cenário guiado envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="129fd-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="129fd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="129fd-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="129fd-107">Introdução</span><span class="sxs-lookup"><span data-stu-id="129fd-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="129fd-108">Noções básicas</span><span class="sxs-lookup"><span data-stu-id="129fd-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="129fd-109">Configuração</span><span class="sxs-lookup"><span data-stu-id="129fd-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="129fd-110">Atribuições</span><span class="sxs-lookup"><span data-stu-id="129fd-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="129fd-111">Análise e criação</span><span class="sxs-lookup"><span data-stu-id="129fd-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="129fd-112">Depois de concluir as etapas do cenário orientado, as políticas do Microsoft Intune habilitarão os seguintes recursos do Microsoft Edge para empresas:</span><span class="sxs-lookup"><span data-stu-id="129fd-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="129fd-113">Identidade dupla</span><span class="sxs-lookup"><span data-stu-id="129fd-113">Dual identity</span></span>
- <span data-ttu-id="129fd-114">Integração com a política de proteção de aplicativos do Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="129fd-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="129fd-115">Integração com o proxy de Aplicativo do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="129fd-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="129fd-116">Favoritos gerenciados e atalhos da página inicial</span><span class="sxs-lookup"><span data-stu-id="129fd-116">Managed favorites and home page shortcuts</span></span>
