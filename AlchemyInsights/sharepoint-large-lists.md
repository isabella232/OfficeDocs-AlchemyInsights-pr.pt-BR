---
title: Listas grandes do SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720121"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="b8319-102">Trabalhar com listas e bibliotecas grandes no SharePoint</span><span class="sxs-lookup"><span data-stu-id="b8319-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="b8319-103">Bibliotecas e listas do SharePoint podem conter até 30 milhões itens, mas quando têm mais de 5.000 itens, você pode ver um erro de limite de exibição de lista quando tenta trabalhar com eles.</span><span class="sxs-lookup"><span data-stu-id="b8319-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="b8319-104">Esse limite serve para manter o desempenho do serviço.</span><span class="sxs-lookup"><span data-stu-id="b8319-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="b8319-105">Ele não pode ser alterado.</span><span class="sxs-lookup"><span data-stu-id="b8319-105">It can't be changed.</span></span> <span data-ttu-id="b8319-106">Para evitar o atingir esse limite:</span><span class="sxs-lookup"><span data-stu-id="b8319-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="b8319-107">**Usar moderno**</span><span class="sxs-lookup"><span data-stu-id="b8319-107">**Use modern**</span></span>

<span data-ttu-id="b8319-108">Modos de exibição mostrando muitos itens funcionam melhor na experiência moderna.</span><span class="sxs-lookup"><span data-stu-id="b8319-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="b8319-109">[Use a experiência moderna](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) para evitar erros que você pode ver na experiência clássica.</span><span class="sxs-lookup"><span data-stu-id="b8319-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="b8319-110">**Adicionar índices**</span><span class="sxs-lookup"><span data-stu-id="b8319-110">**Add indexes**</span></span>

<span data-ttu-id="b8319-111">Ao filtrar ou classificar por uma coluna que não tem um índice, você pode ver uma mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="b8319-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="b8319-112">[Adicione um índice](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manualmente de **configurações de lista** no menu configurações e, em seguida, **colunas indexadas**.</span><span class="sxs-lookup"><span data-stu-id="b8319-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="b8319-113">**Editar o modo de exibição de lista**</span><span class="sxs-lookup"><span data-stu-id="b8319-113">**Edit the list view**</span></span>

<span data-ttu-id="b8319-114">Se ocorrer um erro ao trabalhar com uma lista grande, [edite o modo de exibição de lista](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="b8319-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="b8319-115">As quatro alterações a seguir removerão erros de limite de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="b8319-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="b8319-116">Faça todas as quatro alterações para remover todos os erros.</span><span class="sxs-lookup"><span data-stu-id="b8319-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="b8319-117">Se você ainda estiver recebendo erros, marque [gerenciar grandes listas e bibliotecas](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="b8319-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="b8319-118">Selecione **nenhum** dos dois **primeiros classifique pela coluna** e **, em seguida, classifique pela coluna**.</span><span class="sxs-lookup"><span data-stu-id="b8319-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="b8319-119">Selecione **nenhum** do **primeiro grupo pela coluna** e **, em seguida, agrupe pela coluna**.</span><span class="sxs-lookup"><span data-stu-id="b8319-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="b8319-120">Selecione **nenhum** para todas as colunas na seção **totais** .</span><span class="sxs-lookup"><span data-stu-id="b8319-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="b8319-121">Cancele a seleção de todas, exceto uma coluna para exibição da seção **colunas** .</span><span class="sxs-lookup"><span data-stu-id="b8319-121">Deselect all but one column for display from the **Columns** section.</span></span>

