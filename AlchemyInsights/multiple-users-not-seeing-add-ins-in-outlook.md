---
title: Vários usuários não estão vendo suplementos no Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011792"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Vários usuários não estão vendo suplementos no Outlook

Se você testar suplementos do Outlook e nenhum for exibido, como uma primeira etapa de solução de problemas, use o cmdlet do Windows PowerShell **Get-Set OrganizationConfig** para consultar o parâmetro do _AppsForOfficeEnabled_. Se a consulta retornar um valor **Falso**, defina esse parâmetro como **Verdadeiro** usando o cmdlet **Set-Set OrganizationConfig**, para que os suplementos apareçam como esperado.

Não recomendamos que o parâmetro _AppsForOfficeEnabled_ esteja definido como **False**. Um valor de **False** substitui todas as configurações de função Administrativa e de Usuário acima e impede que novos aplicativos sejam ativados por qualquer usuário na organização.

Para obter mais informações, consulte [Especificar os administradores e usuários que podem instalar e gerenciar suplementos do Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).