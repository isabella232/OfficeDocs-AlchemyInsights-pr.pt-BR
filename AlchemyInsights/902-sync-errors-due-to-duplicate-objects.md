---
title: 902 (erros de sincronização devido aos objetos duplicados)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919860"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="681ac-102">Erros de sincronização devido aos objetos duplicados</span><span class="sxs-lookup"><span data-stu-id="681ac-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="681ac-103">Você pode receber uma das seguintes mensagens de erro quando termina de sincronização de diretórios:</span><span class="sxs-lookup"><span data-stu-id="681ac-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="681ac-104">Não é possível atualizar este objeto no Microsoft Online Services porque os seguintes atributos associados a esse objeto têm valores que já esteja associados a outro objeto em seu diretório local.</span><span class="sxs-lookup"><span data-stu-id="681ac-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="681ac-105">Já existe um objeto sincronizado com o mesmo endereço de proxy em seu diretório do Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="681ac-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="681ac-106">Não é possível atualizar este objeto porque os seguintes atributos associados a esse objeto têm valores que já esteja associados a outro objeto em seus serviços de diretório local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="681ac-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="681ac-107">Para identificar e corrigir o problema, baixe e execute a [Ferramenta de correção de erro do IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="681ac-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="681ac-108">Para obter mais informações, consulte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="681ac-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

