---
title: Criar usuário
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896703"
---
# <a name="create-user"></a>Criar usuário

**COMUNICADO:**

- [Deprecation of WebView sign-in support from Google starting january 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Teste se seus aplicativos podem ser afetados seguindo as [diretrizes do Google](https://go.microsoft.com/fwlink/?linkid=2157323) sobre a compatibilidade de teste.
- Certifique-se de usar o webview do sistema ou o navegador do sistema ao entrar em seus usuários com contas do Google de consumidor. Para obter mais informações, confira [Problemas para entrar nos aplicativos usando apenas o navegador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Não consigo criar um novo usuário no meu Azure Active Directory**

1. Certifique-se de que você está autorizado a criar um novo usuário padrão. Somente o administrador global ou a função de administrador do usuário no Azure Active Directory (AD) podem criar um novo usuário padrão. Se você não estiver em uma dessas funções, peça a um administrador para adicioná-lo a uma dessas funções ou para criar uma nova conta de usuário para você.
1. Certifique-se de que o nome de usuário esteja em um domínio verificado no Azure AD. Se você não tiver nenhum nome de domínio personalizado verificado no seu Azure AD, poderá usar o domínio inicial do Azure AD, que termina com *.onmicrosoft.com.
1. Certifique-se de que o nome de usuário esteja em um domínio não federado ao Azure AD do seu AD local. Os usuários não podem ser adicionados à nuvem com nomes de domínio federados no local.
1. Certifique-se de que nenhum outro usuário ou contato já tenha o nome de usuário que você deseja atribuir ao novo usuário. Os nomes de usuário devem ser exclusivos no Azure AD.
1. Confira as [Funções e administradores do Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para o seu Azure AD.
1. Confira os [nomes de domínio](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para o seu Azure AD.
1. Revise os [logs de auditoria](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para ver informações mais detalhadas sobre um usuário criado ou excluído recentemente, como quem executou a ação e quando.
1. Para obter mais informações sobre como adicionar novos usuários, consulte [Use the Azure portal to create a new user in your Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal).
1. [Funções administrativas do Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Permissões de função de administrador em Azure Active Directory
1. Você também pode [usar o Azure AD PowerShell para criar um novo usuário](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
