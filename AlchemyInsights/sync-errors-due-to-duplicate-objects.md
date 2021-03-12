---
title: 902 (Erros de sincronização devido a objetos duplicados)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708050"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="a3d37-102">Erros de sincronização devido a objetos duplicados</span><span class="sxs-lookup"><span data-stu-id="a3d37-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="a3d37-103">Você pode receber uma das seguintes mensagens de erro quando a sincronização de diretório terminar no Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="a3d37-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="a3d37-104">Não é possível atualizar esse objeto no Microsoft Online Services porque os atributos a seguir associados a esse objeto têm valores que podem já estar associados a outro objeto em seu diretório local.</span><span class="sxs-lookup"><span data-stu-id="a3d37-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="a3d37-105">Um objeto sincronizado com o mesmo endereço proxy já existe no diretório de Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="a3d37-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="a3d37-106">Não é possível atualizar esse objeto porque os atributos a seguir associados a este objeto têm valores que podem já estar associados a outro objeto em seus serviços de diretório local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a3d37-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="a3d37-107">Para identificar e corrigir o problema, baixe e execute a Ferramenta de Correção de Erros do [IdFix DirSync.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="a3d37-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="a3d37-108">Para obter mais informações, consulte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="a3d37-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
