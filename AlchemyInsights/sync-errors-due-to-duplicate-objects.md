---
title: 902 (sincronizar erros devido a objetos duplicados)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767103"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="0cae2-102">Erros de sincronização devido a objetos duplicados</span><span class="sxs-lookup"><span data-stu-id="0cae2-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="0cae2-103">Você pode receber uma das seguintes mensagens de erro quando a sincronização de diretório for concluída no Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="0cae2-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="0cae2-104">Não é possível atualizar esse objeto no Microsoft Online Services porque os seguintes atributos associados a esse objeto têm valores que já podem estar associados a outro objeto no seu diretório local.</span><span class="sxs-lookup"><span data-stu-id="0cae2-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="0cae2-105">Um objeto sincronizado com o mesmo endereço de proxy já existe no diretório do Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="0cae2-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="0cae2-106">Não é possível atualizar esse objeto porque os seguintes atributos associados a esse objeto têm valores que já podem estar associados a outro objeto em seus serviços de diretório local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="0cae2-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="0cae2-107">Para identificar e corrigir o problema, baixe e execute a [ferramenta de correção de erros do IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="0cae2-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="0cae2-108">Para obter mais informações, consulte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="0cae2-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
