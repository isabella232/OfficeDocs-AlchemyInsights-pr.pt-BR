---
title: Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814252"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="b3dee-102">Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios</span><span class="sxs-lookup"><span data-stu-id="b3dee-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="b3dee-103">**Sintoma**</span><span class="sxs-lookup"><span data-stu-id="b3dee-103">**Symptom**</span></span>

<span data-ttu-id="b3dee-104">Os usuários não conseguem abrir relatórios.</span><span class="sxs-lookup"><span data-stu-id="b3dee-104">Users are unable to open reports.</span></span> <span data-ttu-id="b3dee-105">"Algo deu errado.</span><span class="sxs-lookup"><span data-stu-id="b3dee-105">"Something has gone wrong.</span></span> <span data-ttu-id="b3dee-106">Verifique detalhes técnicos para obter mais detalhes."</span><span class="sxs-lookup"><span data-stu-id="b3dee-106">Check technical details for more details."</span></span>

<span data-ttu-id="b3dee-107">**Causa**</span><span class="sxs-lookup"><span data-stu-id="b3dee-107">**Cause**</span></span>

<span data-ttu-id="b3dee-108">Os relatórios não serão carregados no UCI com o erro "O descritor de formulário é nulo ou não definido".</span><span class="sxs-lookup"><span data-stu-id="b3dee-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="b3dee-109">Os relatórios na UCI ainda exigem caixas de diálogo herdadas, nesse caso, o sistema do cliente precisa ter o *allowlegacydialogsembedding* habilitado.</span><span class="sxs-lookup"><span data-stu-id="b3dee-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="b3dee-110">**Solução**</span><span class="sxs-lookup"><span data-stu-id="b3dee-110">**Solution**</span></span>

1. <span data-ttu-id="b3dee-111">Acesse **Configurações > Administração > Configurações do Sistema > Guia Geral**.</span><span class="sxs-lookup"><span data-stu-id="b3dee-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="b3dee-112">Configure "Habilitar a incorporação de determinadas caixas de diálogo herdadas no cliente do navegador da Interface Unificada" para **Sim**.</span><span class="sxs-lookup"><span data-stu-id="b3dee-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
