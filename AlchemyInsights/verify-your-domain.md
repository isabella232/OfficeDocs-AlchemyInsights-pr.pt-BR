---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365405"
---
# <a name="verify-your-domain"></a><span data-ttu-id="dd1fd-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="dd1fd-102">Verify your domain</span></span>

 <span data-ttu-id="dd1fd-103">**O registro provavelmente não foi atualizado na Internet.**</span><span class="sxs-lookup"><span data-stu-id="dd1fd-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="dd1fd-104">Normalmente, apenas alguns minutos levam alguns minutos para que possamos ver o novo registro, mas, ocasionalmente, pode levar algumas horas.</span><span class="sxs-lookup"><span data-stu-id="dd1fd-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="dd1fd-105">Se você já tiver aguardado muito, verifique novamente se copiou e colou o valor exato no registro de verificação TXT no seu host DNS.</span><span class="sxs-lookup"><span data-stu-id="dd1fd-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="dd1fd-106">Um problema comum é não incluir a parte "MS=" no registro.</span><span class="sxs-lookup"><span data-stu-id="dd1fd-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="dd1fd-107">Precisamos disso também!</span><span class="sxs-lookup"><span data-stu-id="dd1fd-107">We need that too!</span></span>

- <span data-ttu-id="dd1fd-108">Em alguns hosts DNS, você pode ter que executar uma etapa extra para salvar o arquivo de zona (local em que o registro DNS é armazenado) para que o registro seja atualizado na Internet.</span><span class="sxs-lookup"><span data-stu-id="dd1fd-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="dd1fd-109">Certifique-se de salvar as alterações para o Office 365 poder ver e verificar o registro.</span><span class="sxs-lookup"><span data-stu-id="dd1fd-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
