---
title: Problemas de gerenciamento de usuários
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 70f8def2a0f3419a9aa6325e376ba52fc35ec48b61f39ede99d7e58cd6c6c464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971436"
---
# <a name="user-management-issues"></a>Problemas de gerenciamento de usuários

**O que acontece com os atuais usuários atribuídos ao aplicativo se eu desabilitar a propriedade ‘Atribuição de usuário necessária’ (definir esta propriedade para Não)?**

Desabilitar **Atribuição de usuário necessária** NÃO afeta os usuários atribuídos atuais. Desabilitar esta propriedade apenas permite que todos os usuários acessem o aplicativo. Todos os usuários listados e aqueles usuários atribuídos a grupos no aplicativo ainda serão válidos.

- Para restringir seu aplicativo a um conjunto específico de usuários, consulte - [Restringir aplicativo do Azure AD a um conjunto específico de usuários - Plataforma de identidade da Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Para atribuir usuários e grupos a aplicativos empresariais no Azure Active Directory (Azure AD), seja a partir do portal do Azure ou usando o PowerShell, consulte [Gerenciar atribuição de usuário para um aplicativo no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Para delegar a criação de aplicativo e permissões de gerenciamento, consulte [Delegar permissões de administrador para gerenciamento de aplicativo - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Ocultar de usuários aplicativos empresariais específicos** - Siga as seguintes etapas para ocultar todos os Microsoft 365 Apps do painel **MyApps**. Os aplicativos ainda estarão visíveis no Portal do Office 365.

 1. Entre no portal do Azure como um administrador global do seu diretório. 
 2. Selecione **Azure Active Directory**. 
 3. Selecione **Usuários**. 
 4. Selecione **Configurações de usuário**. 
 5. Em **aplicativos Enterprise**, clique em **Gerenciar como os usuários finais iniciam e exibem seus aplicativos**. 
 6. Para **Usuários somente podem ver os Office 365 apps no Portal do Office 365**, clique em **Sim**. 
 7. Clique em **Salvar**. 
 8. Para saber mais, consulte [Ocultar um aplicativo Enterprise da experiência do usuário no Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Se você oferecer um aplicativo de Software como Serviço (SaaS) a muitas organizações, você pode configurar seu aplicativo para aceitar entradas a partir de qualquer locatário do Azure Active Directory (Azure AD). Esta configuração é chamada "tornando seu aplicativo multilocatário". Usuários em todos os locatários do Azure AD poderão entrar no seu aplicativo após consentir usar a conta deles com o esse aplicativo. Para mais informações, consulte [Construir aplicativos que conectem usuários do Azure AD - Plataforma de identidade da Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Como um usuário final pode acessar o aplicativo depois que ele(a) tenha sido atribuído(a) ao aplicativo?**

Cada aplicativo numa folha do aplicativo Enterprise tem um link para os usuários finais acessarem. Os usuários também podem acessar o portal **Myapps** de uma forma fácil.

- **Quer saber quais aplicativos e tipos de aplicativos estão sendo usados pelos usuários?**

Você pode baixar relatórios de entrada dos últimos 30 dias do **portal.azure.com > Azure Active directory> Entradas> baixar relatórios**.

- Aprenda como [Conceder a locatário amplo consentimento de administrador a um aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) e [Configurar como usuários finais dão consentimento a aplicativos](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Entenda [como o consentimento funciona](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) e [Gerencie consentimento a aplicativos](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


