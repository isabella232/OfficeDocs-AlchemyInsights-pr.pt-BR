---
title: Criar um site no SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057954"
---
# <a name="create-sharepoint-sites-using-templates"></a>Criar SharePoint sites usando modelos

A capacidade de salvar um site como modelo não é compatível com os Sites de Equipe e Comunicação moderna. Para obter mais informações sobre como usar modelos de site, consulte [Salvar, baixar e carregar um site do SharePoint como um modelo](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Aqui estão alguns problemas/soluções comuns sobre Salvar um Site ou Lista como um modelo no Sharepoint Online. 

**O botão Salvar modelo de site/lista não está disponível ou ausente**

Os administradores devem Permitir o Script Personalizado para habilitar os recursos do modelo. Para etapas detalhadas, exemplos e considerações consulte 

- [Permitir ou impedir o script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- O comando Salvar site como modelo não tem suporte e pode causar problemas em sites que usam a Infraestrutura de Publicação do SharePoint Server.

**O modelo de site não pode ser criado ou não funciona corretamente**

O modelo pode estar faltando [um recurso](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e não será ativado. Se o recurso não estiver disponível para ser ativado no conjunto de sites atual, você não poderá usar o modelo de site para criar um site.

- Verifique se alguma lista ou biblioteca excedeu o [Limite de Modo de Exibição de Lista](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 itens, pois isto pode bloquear a criação de um modelo de site.

- O site pode estar usando muitos recursos e, portanto, o modelo de site ultrapassa o limite de 50 MB.


- Há problemas para exibir os dados de uma lista que usa uma coluna de pesquisa. Para obter mais informações, consulte [Lista gerada pelo modelo não exibe os dados da lista de pesquisa correta no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Para obter informações mais detalhadas sobre problemas e soluções comuns, verifique [Criar e usar modelos de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



