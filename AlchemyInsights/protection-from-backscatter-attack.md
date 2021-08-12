---
title: Proteção contra ataques de Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8c6b1cfe79d322702279877ff351397a366fa246710c04e25181a675ad2fdeab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911218"
---
# <a name="protection-from-backscatter-attack"></a>Proteção contra ataques de Backscatter

Backscatter são notificações de falha na entrega (também conhecidas como notificações de entrega ou mensagens de devolução) que você recebe para mensagens não enviadas. Os remetentes de spam forjam (falsificam) o **De:** endereço de suas mensagens e costumam usar endereços de email reais para dar credibilidade às suas mensagens. Portanto, quando os remetentes de spam inevitavelmente enviam mensagens para destinatários não existentes, o servidor de email de destino é essencialmente enganado para retornar a mensagem não entregue em uma NDR para o remetente forjado no endereço **De:**.

Informações adicionais podem ser encontradas em [Backscatter no EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Habilitar a proteção contra Backscatter**

Para habilitar a proteção contra backscatter, siga o caminho abaixo.

**protection.office.com > Gerenciamento de Ameaças > Política > Antispam > Selecionar a Política de Filtro de Spam e Editar política > Propriedades de spam > Marcar como spam > backscatter de NDR > Definir como "Ativado"**

Se você acredita que uma conta foi comprometida, consulte o seguinte:

- [Responder a uma Conta de Email Comprometida](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Remover usuários bloqueados do portal de Usuários Restritos no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



