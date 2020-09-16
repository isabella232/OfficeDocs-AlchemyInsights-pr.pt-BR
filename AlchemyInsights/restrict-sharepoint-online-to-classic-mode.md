---
title: Restringir o modo clássico do SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751410"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restringir o modo clássico do SharePoint Online

Algumas organizações ainda exigem a experiência de modo clássico. Embora não haja planos de remover o modo clássico em um nível granular, não é mais possível restringir uma organização inteira (locatário) a um modo clássico para listas e bibliotecas.

O administrador terá as seguintes opções para gerenciar listas e bibliotecas individuais no modo clássico usando opções de recusa granular que fornecemos nos seguintes níveis:

- conjunto de sites
- site
- list
- Libra

Além disso, as listas que usam determinados recursos e personalizações que não são suportadas pela moderna ainda serão automaticamente alternadas para o modo clássico.

A partir de 1º de abril de 2019, o processo para desativar o consentimento de nível de locatário de listas e bibliotecas modernas começará e continuará em 31 de maio de 2019.  As listas e bibliotecas que estão no modo clássico como resultado da recusa do locatário serão automaticamente deslocadas para o moderno.

Se você precisar do modo clássico, Confira mais informações [aqui](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) e instruções do PowerShell do PNP [aqui](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) que descrevem as opções e ferramentas que você pode usar atualmente para usar a experiência de modo clássico.
