---
title: Salvar site ou lista como um modelo
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109192"
---
# <a name="save-site-or-list-as-a-template"></a>Salvar site ou lista como um modelo

Os modelos de site do SharePoint são definições pré-compiladas projetadas de acordo com uma necessidade comercial em particular. Para obter mais informações, consulte [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Aqui estão alguns problemas/soluções comuns sobre Como salvar um site ou uma lista como um modelo em SharePoint Online.

O botão Salvar modelo de **site/lista não está disponível ou ausente.** 

- Os administradores devem Permitir o Script Personalizado para habilitar os recursos do modelo. Para etapas detalhadas, exemplos e considerações consulte [Permitir ou impedir script personalizado.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- O comando Salvar site como modelo não tem suporte e pode causar problemas em sites que usam a Infraestrutura de Publicação do SharePoint Server.


**O modelo de site não pode ser criado ou não funciona corretamente**

- O modelo pode estar faltando [um recurso](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não será ativado. Se o recurso não estiver disponível para ser ativado no conjunto de sites atual, você não poderá usar o modelo de site para criar um site.


- Verifique se alguma lista ou biblioteca excedeu o [Limite de Modo de Exibição de Lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 itens, pois isto pode bloquear a criação de um modelo de site.


- O site pode estar usando muitos recursos e, portanto, o modelo de site excede o limite de 50 megabyte (MB).


- Há problemas para exibir os dados de uma lista que usa uma coluna de pesquisa. Para obter mais informações, consulte [Template-generated list does't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Para obter informações mais detalhadas sobre problemas e soluções comuns, faça referência, [Crie e use modelos de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

