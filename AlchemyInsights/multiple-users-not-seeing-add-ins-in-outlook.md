---
title: Vários usuários não estão vendo suplementos no Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154544"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Vários usuários não estão vendo suplementos no Outlook

Se você testar suplementos do Outlook e nenhum for exibido, como uma primeira etapa de solução de problemas, use o cmdlet do Windows PowerShell **Get-Set OrganizationConfig** para consultar o parâmetro do _AppsForOfficeEnabled_. Se a consulta retornar um valor **Falso**, defina esse parâmetro como **Verdadeiro** usando o cmdlet **Set-Set OrganizationConfig**, para que os suplementos apareçam como esperado.

Não é recomendável que o parâmetro _AppsForOfficeEnabled_ esteja definido como **Falso**. Um valor **Falso** substitui todas as configurações de funções administrativas e de usuário acima e impede que os novos aplicativos sejam ativados por qualquer usuário da organização.

Para obter mais informações, consulte [Especificar os administradores e usuários que podem instalar e gerenciar suplementos do Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).