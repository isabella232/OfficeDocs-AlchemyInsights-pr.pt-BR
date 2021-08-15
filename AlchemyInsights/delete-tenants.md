---
title: Excluir locatário
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993881"
---
# <a name="delete-tenant"></a>Excluir locatário

Para excluir um Azure AD, verifique:
- Você é um Administrador Global no diretório.
- Você NÃO está assinado com uma conta que tenha o diretório padrão, como contoso.onmicrosoft.com na conta assinada, como admin@contoso.onmicrosoft.com.
- Remova todos os aplicativos ativos no diretório antes da exclusão. Para remover aplicativos ativos, navegue até Registros de aplicativo e remova os aplicativos existentes.
- Não há assinaturas ativas para Microsoft Online Services, como Microsoft Azure, Office 365 ou Azure AD Premium associados no diretório. Transfira suas assinaturas ou agiliza o cancelamento de assinaturas ativas por meio do Suporte e cobrança do Azure. Saiba mais sobre Como cancelar assinaturas Office 365 e do Azure. Para obter orientações sobre como associar ou adicionar uma assinatura existente a um locatário, consulte [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Não há nenhuma licença ativa. Para remover licenças, consulte [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Não há outros usuários ativos no diretório além de si mesmo como Administrador Global ao tentar excluir o Azure AD. Remova outros usuários ativos e quaisquer dependências de um nome de domínio personalizado no locatário também precisarão ser removidas, como usuários criados com admin@contoso.com.

Para obter mais etapas detalhadas sobre como:
- Exclua "Azure Active Directory" ou "assinatura", consulte [Excluir Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Removendo aplicativos no diretório, consulte [Removendo Aplicativos](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
