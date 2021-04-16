---
title: Gerenciar a lista de endereços global da organização e o catálogo de endereços offline
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
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794820"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Gerenciar a lista de endereços global (LEG) da organização e o catálogo de endereços offline (CEO)

Uma LEG (lista de endereços global) é uma lista de objetos habilitados para e-mail (qualquer tipo de destinatário que possa receber e-mails) na organização. Uma LEG é criada automaticamente em todas as organizações. Você pode criar LEGs adicionais para separar os usuários por organização ou local, mas um único usuário só pode ver e usar uma LEG por vez.

Alguns clientes de e-mail, como o Outlook para Windows, baixam a LEG para uso off-line. Isso é conhecido como um catálogo de endereços offline (CEO). No Exchange Online, um CEO é atualizado apenas uma vez a cada oito horas. em seguida, os clientes devem baixá-lo para atualizar sua cópia do CEO local. Qualquer alteração de destinatário tem que ser visível primeiro na LEG, para que ela seja disponibilizada para o CEO.

Estes são alguns procedimentos que costumam ser usados para a LEG e o CEO:

- Por vários motivos, talvez você queira que alguns objetos sejam ocultados da LEG. Confira [Ocultar destinatários das listas de endereços](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Se você precisar fornecer aos grupos específicos modos de exibição personalizados da LEG da organização, confira [Políticas do catálogo de endereços do Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Criar uma lista de endereços global no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) e aprender a trabalhar com permissões de LEG, confira[Listas de endereços no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Observe que, se você criar uma nova LEG, talvez também queira criar um novo CEO. Consulte [Procedimentos do catálogo de endereços offline](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
