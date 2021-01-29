---
title: Configurar e personalizar aplicativos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50043975"
---
# <a name="configure-and-customize-applications"></a>Configurar e personalizar aplicativos

**Configurar aplicativos**

1. Guia de início rápido: configurar propriedades para um aplicativo em seu locatário do [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) mostra como configurar algumas das propriedades para um aplicativo.
2. Para ajudar a integrar seus aplicativos ao Azure Active Directory, desenvolvemos um conjunto de [tutoriais que](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) o guiam pela configuração.
3. [Como configurar um](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) aplicativo proxy de aplicativo ajuda você a entender como configurar um aplicativo proxy de aplicativo no Azure AD para expor seus aplicativos locais à nuvem.
4. [Baixe o PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)e configure seu aplicativo: siga as instruções em Configurar *o PingAccess para Azure AD* para proteger aplicativos publicados usando o Proxy de Aplicativo do Microsoft Azure AD no site identidade de ping e baixe a versão mais recente do PingAccess.

**Erros de aplicativo configurado indefigurado (AADSTS650056)**

1. Verifique se você está acessando o aplicativo a partir do endereço de entrada fornecido pelo proprietário do aplicativo. Caso contrário, entre no aplicativo por meio de seu processo normal. Na maioria dos casos, isso será resolvido automaticamente naturalmente. Se isso não for o caso, esta postagem pode ajudar a solucionar problemas e resolvê-la.
2. **Se a sua organização possui o aplicativo** (ou seja, o registro do aplicativo está em sua organização):
    - No mínimo, recomendamos que a `User.Read` permissão `openid` ou delegada do Microsoft **Graph** seja adicionada.
    - Certifique-se de que o aplicativo e todas as suas permissões sejam consentida. Você pode verificar isso analisando a coluna **Status** do registro do aplicativo nas **permissões da API.**
    - Em alguns cenários, o aplicativo pode ser de terceiros, no entanto, ele pode ser registrado em sua organização. Confirme se esse aplicativo está listado em seus registros de aplicativo (aplicativos não empresariais).
    - Se você continuar a ver essa mensagem de erro. Em seguida, talvez seja necessário criar a URL de consentimento descrita na **etapa 4.**
3. **Se sua organização não for o proprietário do aplicativo e usá-la como um aplicativo de terceiros:**
    - Se você for o administrador global/da empresa, deverá ver a tela de consentimento. Marque a caixa "Consentimento **em nome da sua organização".**
    - Se você não vir a tela de consentimento, exclua o aplicativo Enterprise e tente novamente.
    - Se você continuar a ver essa mensagem de erro. Em seguida, talvez seja necessário criar a URL de consentimento descrita na **etapa 4.**
4. **Crie manualmente** a URL de consentimento a ser usada: se o aplicativo for projetado para acessar um recurso específico, talvez você não consiga usar os botões de consentimento do portal do Azure, precisará gerar manualmente sua própria URL de consentimento e usá-la.
    - Você precisará obter o `{App-Id}` e o do proprietário do `{App-Uri-Id}` aplicativo. `{Tenant-Id}` será seu identificador de locatário. Isso será ou `yourdomain.onmicrosoft.com` sua ID de diretório.
    - Se o aplicativo estiver acessando a si mesmo para o recurso, `{App-Id}` o e será o `{App-Uri-Id}` mesmo.
5. Para obter mais informações, consulte Problemas ao entrar em aplicativos configurados com base em [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Personalizar aplicativos**

- Adicione identidade visual à página de login do [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) da sua organização: use o logotipo da sua organização e esquemas de cores personalizados para fornecer uma aparência consistente para as páginas de login do Azure Active Directory (Azure AD).
- Adicione seu nome de domínio personalizado usando o [portal do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – cada novo locatário do Azure AD vem com um nome de domínio inicial. Não é possível alterar ou excluir o nome de domínio inicial, mas você pode adicionar os nomes da sua organização. Adicionar nomes de domínio personalizados ajuda você a criar nomes de usuário que são familiares para seus usuários.
