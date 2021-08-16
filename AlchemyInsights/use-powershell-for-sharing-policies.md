---
title: Usar o Windows PowerShell para Políticas de Compartilhamento e Relações da Organização
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998454"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Usar o Windows PowerShell para Políticas de Compartilhamento e Relações da Organização


Para Relações de organização, examine as informações detalhadas sobre a sintaxe e os parâmetros de: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) e [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Para criar uma política de compartilhamento, use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Para [aplicar uma política de compartilhamento a uma caixa de correio ou usuário](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) você precisa usar uma combinação de [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) e [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) com a política recém-criada. Para [modificar, desabilitar ou remover uma política de compartilhamento](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) você precisa usar [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) e [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Para obter o conhecimento completo deste tópico, leia:**

[Compartilhando no Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)