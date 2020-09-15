---
title: Excluir um usuário órfão do servidor local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680123"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Excluir um usuário órfão do servidor local

Para remover um usuário órfão, siga as etapas a seguir:

1. Force a sincronização de diretórios seguindo as instruções do artigo [O que é identidade híbrida com o Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Para verificar a sincronização de diretórios, confira o artigo [O que é identidade híbrida com o Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Se a sincronização funcionar corretamente, mas a exclusão do objeto Active Directory não for propagada para o Azure AD, remova manualmente o objeto órfão usando um dos seguintes cmdlets do Azure Active Directory para o Windows PowerShell:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Por exemplo, para remover a ID do usuário órfão john.smith@contoso.com, criada originalmente usando a sincronização de diretórios, execute o cmdlet:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com