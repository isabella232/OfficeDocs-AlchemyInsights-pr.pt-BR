---
title: SharePoint listas grandes
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
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941551"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Trabalhar com listas e bibliotecas grandes em SharePoint

SharePoint listas e bibliotecas podem conter até 30 milhões de itens, mas quando eles têm mais de 5.000 itens, você pode ver um erro limite de exibição de lista ao tentar trabalhar com eles. Esse limite serve para manter o desempenho do serviço. Ele não pode ser alterado. Para evitar atingir esse limite:

**Usar moderno**

As exibições mostrando muitos itens funcionam melhor na experiência moderna. [Use a experiência moderna](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) para evitar erros que você pode ver na experiência clássica.

**Adicionar índices**

Ao filtrar ou classificar por uma coluna que não tenha um índice, você pode ver uma mensagem de erro. [Adicione um índice](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manualmente **de Lista Configurações** no menu configurações e, em seguida, **Colunas Indexadas.**

**Editar o modo de exibição de lista**

Se ocorrer um erro ao trabalhar com uma lista grande, [edite seu modo de exibição de lista](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

As quatro alterações a seguir removerão erros de limite de exibição de lista. Faça todas as quatro alterações para remover todos os erros. Se você ainda estiver recebendo erros, verifique [Gerenciar listas e bibliotecas grandes.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Selecione **Nenhum** na **primeira classificação pela coluna** **e, em seguida, classificar pela coluna**.
2. Selecione **Nenhum** no **primeiro grupo pela coluna e,** **em seguida, agrupar pela coluna**.
3. Selecione **Nenhum** para todas as colunas na **seção Totais.**
4. Desmarque todas as colunas, menos uma para exibição na **seção Colunas.**

