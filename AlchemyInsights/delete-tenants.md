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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477641"
---
# <a name="delete-tenant"></a>Excluir locatário

Para excluir um Azure AD, verifique se:
- Você é um administrador global no diretório.
- Você não está conectado com uma conta que tenha o diretório padrão como contoso.onmicrosoft.com na conta de entrada, como admin@contoso.onmicrosoft.com.
- Remova quaisquer aplicativos ativos no diretório antes da exclusão. Para remover aplicativos ativos, navegue até registros de aplicativos e remova os aplicativos existentes.
- Não há assinaturas ativas para os serviços online da Microsoft, como o Microsoft Azure, o Office 365 ou o Azure AD Premium associado ao diretório. Transferir suas assinaturas ou agilizar o cancelamento de assinaturas ativas por meio de suporte e cobrança do Azure. Saiba mais sobre como cancelar assinaturas do Office 365 e do Azure. Para obter orientação sobre como associar ou adicionar uma assinatura existente a um locatário, confira [associar ou adicionar uma assinatura do Azure ao seu locatário do Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Não há licença ativa. Para remover licenças, consulte [How to remove Subscription for remove License](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Não há outros usuários ativos no diretório, além de ser o administrador global ao tentar excluir o Azure AD. Remova outros usuários ativos, e quaisquer dependências em um nome de domínio personalizado no locatário também precisarão ser removidas, como os usuários criados com o admin@contoso.com.

Para obter mais detalhes sobre como:
- Delete "Azure Active Directory" ou "Subscription", consulte [delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Removendo aplicativos no diretório, consulte [removendo aplicativos](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
