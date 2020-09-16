---
title: Gerenciar a lista de endereços global da organização e o catálogo de endereços offline
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a15864f34433695b61ea040abd3032d234920653
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812679"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="3f30a-102">Gerenciar a lista de endereços global (LEG) da organização e o catálogo de endereços offline (CEO)</span><span class="sxs-lookup"><span data-stu-id="3f30a-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="3f30a-103">Uma LEG (lista de endereços global) é uma lista de objetos habilitados para e-mail (qualquer tipo de destinatário que possa receber e-mails) na organização.</span><span class="sxs-lookup"><span data-stu-id="3f30a-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="3f30a-104">Uma LEG é criada automaticamente em todas as organizações.</span><span class="sxs-lookup"><span data-stu-id="3f30a-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="3f30a-105">Você pode criar LEGs adicionais para separar os usuários por organização ou local, mas um único usuário só pode ver e usar uma LEG por vez.</span><span class="sxs-lookup"><span data-stu-id="3f30a-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="3f30a-106">Alguns clientes de e-mail, como o Outlook para Windows, baixam a LEG para uso off-line.</span><span class="sxs-lookup"><span data-stu-id="3f30a-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="3f30a-107">Isso é conhecido como um catálogo de endereços offline (CEO).</span><span class="sxs-lookup"><span data-stu-id="3f30a-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="3f30a-108">No Exchange Online, um CEO é atualizado apenas uma vez a cada oito horas. em seguida, os clientes devem baixá-lo para atualizar sua cópia do CEO local.</span><span class="sxs-lookup"><span data-stu-id="3f30a-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="3f30a-109">Qualquer alteração de destinatário tem que ser visível primeiro na LEG, para que ela seja disponibilizada para o CEO.</span><span class="sxs-lookup"><span data-stu-id="3f30a-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="3f30a-110">Estes são alguns procedimentos que costumam ser usados para a LEG e o CEO:</span><span class="sxs-lookup"><span data-stu-id="3f30a-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="3f30a-111">Por vários motivos, talvez você queira que alguns objetos sejam ocultados da LEG.</span><span class="sxs-lookup"><span data-stu-id="3f30a-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="3f30a-112">Confira [Ocultar destinatários das listas de endereços](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="3f30a-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="3f30a-113">Se você precisar fornecer aos grupos específicos modos de exibição personalizados da LEG da organização, confira [Políticas do catálogo de endereços do Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="3f30a-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="3f30a-114">[Criar uma lista de endereços global no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) e aprender a trabalhar com permissões de LEG, confira[Listas de endereços no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="3f30a-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="3f30a-115">Observe que, se você criar uma nova LEG, talvez também queira criar um novo CEO.</span><span class="sxs-lookup"><span data-stu-id="3f30a-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="3f30a-116">Consulte [Procedimentos do catálogo de endereços offline](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="3f30a-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
