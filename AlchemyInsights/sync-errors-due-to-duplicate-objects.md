---
title: 902 (sincronizar erros devido a objetos duplicados)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859092"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erros de sincronização devido a objetos duplicados

Você pode receber uma das seguintes mensagens de erro quando a sincronização de diretório for concluída:

- Não é possível atualizar esse objeto no Microsoft Online Services porque os seguintes atributos associados a esse objeto têm valores que já podem estar associados a outro objeto no seu diretório local.

- Um objeto sincronizado com o mesmo endereço de proxy já existe no diretório do Microsoft Online Services.

- Não é possível atualizar esse objeto porque os seguintes atributos associados a esse objeto têm valores que já podem estar associados a outro objeto em seus serviços de diretório local: UserPrincipalName.

Para identificar e corrigir o problema, baixe e execute a [ferramenta de correção de erros do IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Para obter mais informações, consulte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
