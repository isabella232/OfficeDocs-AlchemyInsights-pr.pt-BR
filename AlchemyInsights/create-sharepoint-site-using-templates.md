---
title: Criar um site no SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770411"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="83d2e-102">Criar sites do SharePoint usando modelos</span><span class="sxs-lookup"><span data-stu-id="83d2e-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="83d2e-103">A capacidade de salvar um site como modelo não é suportada com a comunicação moderna ou com sites de equipe.</span><span class="sxs-lookup"><span data-stu-id="83d2e-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="83d2e-104">Para obter mais informações sobre como usar modelos [, consulte salvar, baixar e carregar um site do SharePoint como um modelo](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="83d2e-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="83d2e-105">Aqui estão alguns problemas comuns/soluções sobre como salvar um site ou uma lista como um modelo no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="83d2e-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="83d2e-106">**O botão salvar site/modelo de lista não está disponível ou ausente**</span><span class="sxs-lookup"><span data-stu-id="83d2e-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="83d2e-107">Os administradores precisarão permitir que o script personalizado habilite os recursos do modelo.</span><span class="sxs-lookup"><span data-stu-id="83d2e-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="83d2e-108">Para obter etapas detalhadas, exemplos e considerações, consulte</span><span class="sxs-lookup"><span data-stu-id="83d2e-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="83d2e-109">Permitir ou impedir o script personalizado</span><span class="sxs-lookup"><span data-stu-id="83d2e-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="83d2e-110">O comando salvar site como modelo não é suportado e pode causar problemas em sites que usam a infraestrutura de publicação do SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="83d2e-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="83d2e-111">**O modelo de site não pode ser criado ou não funciona corretamente**</span><span class="sxs-lookup"><span data-stu-id="83d2e-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="83d2e-112">O modelo pode não ter um [recurso](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não será ativado.</span><span class="sxs-lookup"><span data-stu-id="83d2e-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="83d2e-113">Se o recurso não estiver disponível para ser ativado no conjunto de sites atual, você não poderá usar o modelo de site para criar um site.</span><span class="sxs-lookup"><span data-stu-id="83d2e-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="83d2e-114">Verifique se as listas ou bibliotecas excedem o limite de [exibição de lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 itens, pois isso pode bloquear a criação de um modelo de site.</span><span class="sxs-lookup"><span data-stu-id="83d2e-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="83d2e-115">O site pode estar usando muitos recursos e, portanto, o modelo de site excede o limite de 50 MB.</span><span class="sxs-lookup"><span data-stu-id="83d2e-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="83d2e-116">Há problemas ao exibir dados de uma lista que usa uma coluna de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="83d2e-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="83d2e-117">Para obter mais informações, consulte [Template-generated List não exibe dados da lista de pesquisa correta no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="83d2e-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="83d2e-118">Para obter informações mais detalhadas sobre problemas e soluções comuns, verifique [criar e usar modelos de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="83d2e-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



