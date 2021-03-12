---
title: Solucionar problemas de instalação do MDATP em um Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735415"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="983a9-102">Solucionar problemas de instalação do MDATP em um Mac</span><span class="sxs-lookup"><span data-stu-id="983a9-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="983a9-103">Se a instalação manual falhar, a página **Resumo** do assistente de instalação mostrará o seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="983a9-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="983a9-104">"Ocorreu um erro durante a instalação.</span><span class="sxs-lookup"><span data-stu-id="983a9-104">"An error occurred during installation.</span></span> <span data-ttu-id="983a9-105">O Instalador encontrou um erro que causou a falha da instalação.</span><span class="sxs-lookup"><span data-stu-id="983a9-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="983a9-106">Entre em contato com o fabricante do software para assistência."</span><span class="sxs-lookup"><span data-stu-id="983a9-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="983a9-107">Para implantações MDM, a página também mostra uma falha de instalação genérica.</span><span class="sxs-lookup"><span data-stu-id="983a9-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="983a9-108">Embora não exibemos erros exatos para os usuários finais, manteremos um arquivo de log com progresso de instalação, em **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="983a9-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="983a9-109">Cada sessão de instalação é anexada a esse arquivo de log.</span><span class="sxs-lookup"><span data-stu-id="983a9-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="983a9-110">Para saída somente da última sessão de instalação, use `sed` .</span><span class="sxs-lookup"><span data-stu-id="983a9-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="983a9-111">Para saber mais, confira [Solucionar problemas de instalação do Microsoft Defender ATP para Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="983a9-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
