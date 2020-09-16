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
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="00c06-102">Vários objetos têm o mesmo endereço de email que a identidade</span><span class="sxs-lookup"><span data-stu-id="00c06-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="00c06-103">**Vários objetos**</span><span class="sxs-lookup"><span data-stu-id="00c06-103">**Multiple objects**</span></span>

<span data-ttu-id="00c06-104">Uma das razões comuns desse erro é não ser possível rotear uma solicitação do Outlook Web Access corretamente em uma presença de vários objetos com o mesmo endereço de email que a identidade.</span><span class="sxs-lookup"><span data-stu-id="00c06-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="00c06-105">Para encontrar esses objetos, execute os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="00c06-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="00c06-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="00c06-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="00c06-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="00c06-107">· Get-User <email address></span></span>

<span data-ttu-id="00c06-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="00c06-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="00c06-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="00c06-109">· Get-Contact <email address></span></span>

<span data-ttu-id="00c06-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="00c06-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="00c06-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="00c06-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="00c06-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="00c06-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="00c06-113">Para resolver o problema, remova vários objetos com a mesma identidade de email e verifique se há um único objeto com a identidade de email específica e se o tipo de destinatário é UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="00c06-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="00c06-114">**O mesmo endereço é usado para caixas de correio comerciais e de consumo**</span><span class="sxs-lookup"><span data-stu-id="00c06-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="00c06-115">O mesmo endereço é usado para caixas de correio comerciais e de consumo.</span><span class="sxs-lookup"><span data-stu-id="00c06-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="00c06-116">Nesse caso, o usuário deve alterar seu alias de consumidor principal até que o Cafe dê suporte a esse cenário.</span><span class="sxs-lookup"><span data-stu-id="00c06-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="00c06-117">Esse é um erro permanente que não desaparece sem intervenção.</span><span class="sxs-lookup"><span data-stu-id="00c06-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="00c06-118">Para obter detalhes, confira [Alterar o número de telefone ou endereço de email da sua conta Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="00c06-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>