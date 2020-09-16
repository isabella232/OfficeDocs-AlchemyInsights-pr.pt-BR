---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734294"
---
# <a name="verify-your-domain"></a><span data-ttu-id="de6c1-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="de6c1-102">Verify your domain</span></span>

 <span data-ttu-id="de6c1-103">**O registro provavelmente não foi atualizado na Internet.**</span><span class="sxs-lookup"><span data-stu-id="de6c1-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="de6c1-104">Normalmente, apenas alguns minutos levam alguns minutos para que possamos ver o novo registro, mas, ocasionalmente, pode levar algumas horas.</span><span class="sxs-lookup"><span data-stu-id="de6c1-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="de6c1-105">Se você já tiver aguardado muito, verifique novamente se copiou e colou o valor exato no registro de verificação TXT no seu host DNS.</span><span class="sxs-lookup"><span data-stu-id="de6c1-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="de6c1-106">Um problema comum é não incluir a parte "MS=" no registro.</span><span class="sxs-lookup"><span data-stu-id="de6c1-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="de6c1-107">Precisamos disso também!</span><span class="sxs-lookup"><span data-stu-id="de6c1-107">We need that too!</span></span>

- <span data-ttu-id="de6c1-108">Em alguns hosts DNS, você pode ter que executar uma etapa extra para salvar o arquivo de zona (local em que o registro DNS é armazenado) para que o registro seja atualizado na Internet.</span><span class="sxs-lookup"><span data-stu-id="de6c1-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="de6c1-109">Certifique-se de ter salvo suas alterações para que a Microsoft possa ver e verificar o registro.</span><span class="sxs-lookup"><span data-stu-id="de6c1-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
