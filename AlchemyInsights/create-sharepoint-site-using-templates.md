---
title: Criar um site no SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 2097933dd20f326a7bda2151596d514c37d566ff
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717755"
---
# <a name="create-sharepoint-sites-using-templates"></a>Criar sites do SharePoint usando modelos

Os modelos de site do SharePoint são definições pré-compiladas projetadas de acordo com uma necessidade comercial em particular. Para obter mais informações, consulte <a href="https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4">usando modelos para criar diferentes tipos de sites do SharePoint.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Aqui estão alguns problemas comuns/soluções sobre como salvar um site ou uma lista como um modelo no SharePoint Online.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">O botão salvar site/modelo de lista não está disponível ou ausente.</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Os administradores precisarão permitir que o script personalizado habilite os recursos do modelo. Para obter etapas detalhadas, exemplos e considerações, consulte </span> </span> <a style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">permitir ou impedir o script personalizado</a>.</li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">O comando salvar site como modelo não é suportado e pode causar problemas em sites que usam a infraestrutura de publicação do SharePoint Server.</span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">O modelo de site não pode ser criado ou não funciona corretamente</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">É possível que o modelo não <a href="https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx"></a> tenha um recurso&rsquo;e ganha a ativação. Se o recurso não estiver disponível para ser ativado no conjunto de sites atual, você não poderá usar o modelo de site para criar um site.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Verifique se as listas ou bibliotecas excedem o limite <a href="https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59">de exibição de lista de</a> 5000 itens, pois isso pode bloquear a criação de um modelo de site.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">O site pode estar usando muitos recursos e, portanto, o modelo de site excede o limite de 50 MB.</span></li> <li>
Há problemas ao exibir dados de uma lista que usa uma coluna de pesquisa. Para obter mais informações, </span> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> <a style="box-sizing: border-box; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a"> <span style="color: #0067b8; text-decoration: none; text-underline: none;">consulte template-generated List&rsquo;não exibe dados da lista de pesquisa correta no SharePoint Online.

Para obter informações mais detalhadas sobre problemas e soluções comuns, verifique <a href="https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989">criar e usar modelos de site.



