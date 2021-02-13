---
title: Adicionar Microsoft Edge ao Microsoft Intune
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
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177984"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="ddab4-102">Adicionar Microsoft Edge ao Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ddab4-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="ddab4-103">Para poder implantar, configurar, monitorar e proteger o Microsoft Edge para Windows 10, você deve primeiro adicioná-lo ao Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="ddab4-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="ddab4-104">O Intune oferece suporte ao Microsoft Edge 77 e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="ddab4-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="ddab4-105">O Intune detectará todas as instalações pré-existentes do Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="ddab4-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="ddab4-106">Se o Microsoft Edge for instalado no contexto do usuário, uma instalação do sistema substituirá a instalação no contexto do usuário.</span><span class="sxs-lookup"><span data-stu-id="ddab4-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="ddab4-107">Se o Microsoft Edge estiver instalado no contexto do sistema, o sucesso da instalação será relatado.</span><span class="sxs-lookup"><span data-stu-id="ddab4-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="ddab4-108">O Microsoft Edge 77 pré-instalado e versões posteriores, para todos os canais no contexto do usuário, serão substituídos pelo Microsoft Edge instalado no contexto do sistema.</span><span class="sxs-lookup"><span data-stu-id="ddab4-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="ddab4-109">**Pré-requisito**</span><span class="sxs-lookup"><span data-stu-id="ddab4-109">**Prerequisite**</span></span>

<span data-ttu-id="ddab4-110">Windows 10 versão 1709 ou versões posteriores</span><span class="sxs-lookup"><span data-stu-id="ddab4-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="ddab4-111">**Etapas para adicionar o Edge ao Intune**</span><span class="sxs-lookup"><span data-stu-id="ddab4-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="ddab4-112">[Configure o aplicativo no Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="ddab4-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="ddab4-113">[Configure as informações do aplicativo](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="ddab4-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="ddab4-114">[Defina as configurações do aplicativo](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="ddab4-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="ddab4-115">[Selecione os rótulos de escopo (opcional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="ddab4-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="ddab4-116">[Adicione o aplicativo](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="ddab4-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="ddab4-117">Para obter mais ajuda, confira [Solução de problemas](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="ddab4-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




