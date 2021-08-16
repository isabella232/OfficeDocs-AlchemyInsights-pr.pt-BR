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
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011900"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Vários objetos têm o mesmo endereço de email que a identidade

**Vários objetos**

Um dos motivos comuns desse erro é não poder rotear uma solicitação do Outlook Acesso via Web corretamente na presença de vários objetos com o mesmo endereço de email que a identidade. Para localizar esses objetos, execute os seguintes comandos:

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