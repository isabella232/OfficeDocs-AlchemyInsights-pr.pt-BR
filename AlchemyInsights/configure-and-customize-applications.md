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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044976"
---
# <a name="configure-and-customize-applications"></a>Configurar e personalizar aplicativos

**Configurar aplicativos**

1. Início rápido: configurar propriedades para um aplicativo em seu [locatário do Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) mostra como configurar algumas das propriedades para um aplicativo.
2. Para ajudar a integrar seus aplicativos com Azure Active Directory, desenvolvemos uma coleção [de tutoriais](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) que o guiam pela configuração.
3. [Como configurar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) um aplicativo Proxy de Aplicativo ajuda você a entender como configurar um aplicativo Proxy de Aplicativo no Azure AD para expor seus aplicativos locais à nuvem.
4. [Baixe PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)e configure seu aplicativo : siga as instruções em *Configure PingAccess for Azure AD* para proteger aplicativos publicados usando o proxy de aplicativos Microsoft Azure AD no site identidade de ping e baixe a versão mais recente do PingAccess.

**Erros de aplicativo configurado errado (AADSTS650056)**

1. Verifique se você está acessando o aplicativo a partir do endereço de entrada fornecido pelo proprietário do aplicativo. Caso contrário, entre no aplicativo por meio de seu processo normal. Na maioria dos casos, isso será resolvido automaticamente naturalmente. Se não for, essa postagem poderá ajudar a solucionar problemas e resolvê-la.
2. **Se sua organização for proprietária do aplicativo** (o que significa que o registro do aplicativo está em sua organização):
    - No mínimo, recomendamos que a permissão ou delegada da `User.Read` Microsoft `openid` **Graph** seja adicionada.
    - Certifique-se de que o aplicativo e todas as suas permissões sejam consentida. Você pode verificar isso analisando a coluna **Status** do registro do aplicativo em **Permissões de API**.
    - Em alguns cenários, o aplicativo pode ser de terceiros, no entanto, ele pode ser registrado em sua organização. Confirme se esse aplicativo está listado nos registros do aplicativo (não Enterprise aplicativos).
    - Se você continuar a ver essa mensagem de erro. Em seguida, talvez seja necessário criar a URL de consentimento descrita na **etapa 4**.
3. **Se sua organização não for o proprietário do aplicativo e usá-lo como um aplicativo de terceiros**:
    - Se você for o administrador Global/Company, deverá ver a tela de consentimento. Verifique a caixa "Consentimento **em nome da sua organização"**.
    - Se você não vir a tela de consentimento, exclua o aplicativo Enterprise e tente novamente.
    - Se você continuar a ver essa mensagem de erro. Em seguida, talvez seja necessário criar a URL de consentimento descrita na **etapa 4**.
4. **Criar manualmente** a URL de consentimento a ser usada : se o aplicativo for projetado para acessar um recurso específico, talvez você não consiga usar os botões consentimento do portal do Azure, você precisará gerar manualmente sua própria URL de consentimento e usá-la.
    - Você precisará obter o `{App-Id}` e o do proprietário do `{App-Uri-Id}` aplicativo. `{Tenant-Id}` será seu identificador de locatário. Isso será ou `yourdomain.onmicrosoft.com` sua ID de diretório.
    - Se o aplicativo estiver acessando a si mesmo para o recurso, o `{App-Id}` e `{App-Uri-Id}` será o mesmo.
5. Para obter mais informações, consulte Problemas ao entrar em aplicativos configurados com base em [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Personalizar aplicativos**

- [Adicionar](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) identidade visual à página de Azure Active Directory de logona da sua organização - Use o logotipo da sua organização e esquemas de cores personalizados para fornecer uma aparência consistente às páginas de login do Azure Active Directory (Azure AD).
- [Adicione seu nome de domínio personalizado usando o portal Azure Active Directory -](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) Cada novo locatário do Azure AD vem com um nome de domínio inicial. Você não pode alterar ou excluir o nome de domínio inicial, mas pode adicionar os nomes da sua organização. Adicionar nomes de domínio personalizados ajuda você a criar nomes de usuário que são familiares aos seus usuários.
