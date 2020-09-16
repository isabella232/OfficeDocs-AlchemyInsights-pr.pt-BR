---
title: Vários objetos têm o mesmo endereço de email que a identidade
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724603"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Vários objetos têm o mesmo endereço de email que a identidade

**Vários objetos**

Uma das razões comuns desse erro é não ser possível rotear uma solicitação do Outlook Web Access corretamente em uma presença de vários objetos com o mesmo endereço de email que a identidade. Para encontrar esses objetos, execute os seguintes comandos:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Para resolver o problema, remova vários objetos com a mesma identidade de email e verifique se há um único objeto com a identidade de email específica e se o tipo de destinatário é UserMailbox.

**O mesmo endereço é usado para caixas de correio comerciais e de consumo**

O mesmo endereço é usado para caixas de correio comerciais e de consumo. Nesse caso, o usuário deve alterar seu alias de consumidor principal até que o Cafe dê suporte a esse cenário. Esse é um erro permanente que não desaparece sem intervenção.

Para obter detalhes, confira [Alterar o número de telefone ou endereço de email da sua conta Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).