---
title: Não é possível excluir itens em SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038505"
---
# <a name="unable-to-delete-items"></a>Não é possível excluir itens

- As políticas de retenção podem causar isso, você precisa desabilitar ou excluir a respectiva retenção que está causando esse problema. Depois que uma política de retenção ou retenção é removida, pode levar até 24 horas para que a alteração entre em vigor. Verifique se não há uma [configuração de política de](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) retenção no item.

- O site pode ter excedido o limite de armazenamento, aumentar a [cota de site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) e excluir o item.

- Verifique se o item não [foi verificado](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) para outro usuário.

- Por fim, os administradores podem usar SharePoint [Padrões](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) e Práticas (PnP) que contém uma biblioteca de comandos do PowerShell que permitem executar ações de gerenciamento complexas, como forçar a exclusão de itens obstinados.
- [Remover arquivo PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Remover pasta PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Remover Item de Lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Remover lista PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Remover Campo PNP (Coluna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)