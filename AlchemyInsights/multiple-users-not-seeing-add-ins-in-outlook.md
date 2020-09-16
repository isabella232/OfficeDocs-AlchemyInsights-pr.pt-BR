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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729859"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Vários usuários não estão vendo suplementos no Outlook

Se você testar suplementos do Outlook e nenhum for exibido, como uma primeira etapa de solução de problemas, use o cmdlet do Windows PowerShell **Get-Set OrganizationConfig** para consultar o parâmetro do _AppsForOfficeEnabled_. Se a consulta retornar um valor **Falso**, defina esse parâmetro como **Verdadeiro** usando o cmdlet **Set-Set OrganizationConfig**, para que os suplementos apareçam como esperado.

Não é recomendável que o parâmetro _AppsForOfficeEnabled_ esteja definido como **Falso**. Um valor **Falso** substitui todas as configurações de funções administrativas e de usuário acima e impede que os novos aplicativos sejam ativados por qualquer usuário da organização.

Para obter mais informações, consulte [Especificar os administradores e usuários que podem instalar e gerenciar suplementos do Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).