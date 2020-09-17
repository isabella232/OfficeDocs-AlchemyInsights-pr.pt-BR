---
title: Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806423"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="a5d97-102">Habilitar a incorporação de caixas de diálogo herdadas para abrir relatórios</span><span class="sxs-lookup"><span data-stu-id="a5d97-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="a5d97-103">**Sintoma**</span><span class="sxs-lookup"><span data-stu-id="a5d97-103">**Symptom**</span></span>

<span data-ttu-id="a5d97-104">Os usuários não conseguem abrir relatórios.</span><span class="sxs-lookup"><span data-stu-id="a5d97-104">Users are unable to open reports.</span></span> <span data-ttu-id="a5d97-105">"Algo deu errado.</span><span class="sxs-lookup"><span data-stu-id="a5d97-105">"Something has gone wrong.</span></span> <span data-ttu-id="a5d97-106">Verifique detalhes técnicos para obter mais detalhes."</span><span class="sxs-lookup"><span data-stu-id="a5d97-106">Check technical details for more details."</span></span>

<span data-ttu-id="a5d97-107">**Causa**</span><span class="sxs-lookup"><span data-stu-id="a5d97-107">**Cause**</span></span>

<span data-ttu-id="a5d97-108">Os relatórios não serão carregados no UCI com o erro "O descritor de formulário é nulo ou não definido".</span><span class="sxs-lookup"><span data-stu-id="a5d97-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="a5d97-109">Os relatórios na UCI ainda exigem caixas de diálogo herdadas, nesse caso, o sistema do cliente precisa ter o *allowlegacydialogsembedding* habilitado.</span><span class="sxs-lookup"><span data-stu-id="a5d97-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="a5d97-110">**Solução**</span><span class="sxs-lookup"><span data-stu-id="a5d97-110">**Solution**</span></span>

1. <span data-ttu-id="a5d97-111">Acesse **Configurações > Administração > Configurações do Sistema > Guia Geral**.</span><span class="sxs-lookup"><span data-stu-id="a5d97-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="a5d97-112">Configure "Habilitar a incorporação de determinadas caixas de diálogo herdadas no cliente do navegador da Interface Unificada" para **Sim**.</span><span class="sxs-lookup"><span data-stu-id="a5d97-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
