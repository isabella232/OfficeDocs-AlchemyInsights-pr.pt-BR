---
title: Problemas contínuos de login do usuário do SSO
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919195"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problemas contínuos de login do usuário do SSO

Depois que o usuário for autenticado, o navegador armazenará em cache as credenciais do usuário para que, no mesmo navegador, o aplicativo entre automaticamente com a mesma conta. Isso pode dificultar que outro usuário ou um único usuário faça logoff em várias contas em um dispositivo. Para resolver isso: 1. Tente entrar em outro navegador. 2. Limpe o cache e/ou cookies do navegador e tente entrar novamente.

Se você ainda estiver enfrentando problemas de login, recomendamos o seguinte para diagnosticar e automatizar as etapas de resolução:

1. Instale a [Extensão](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) de Navegador Seguro de Meus Aplicativos para ajudar o Azure Active Directory (Azure AD) a fornecer melhores diagnósticos e resoluções ao usar a experiência de teste no portal do Azure.
2. Reproduza o erro usando a experiência de teste na página de configuração do aplicativo no portal do Azure. Para saber mais, consulte Depurar aplicativos de login único [baseados em SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Se você usar a experiência de teste no portal do Azure com a Extensão do Navegador Seguro meus Aplicativos, ignore **a etapa 4.**
4. Para abrir a página de configuração de single sign-on com base em SAML:
    - Abra o [portal do Azure](https://portal.azure.com/) e entre como Administrador **Global** ou **Coadmin.**
    - Abra a **Extensão do Azure Active Directory** selecionando **Todos** os serviços na parte superior do menu de navegação principal do lado esquerdo.
    - Digite "Azure Active Directory" na caixa de pesquisa de filtro e selecione o item **do Azure Active Directory.**
    - Selecione **Aplicativos Empresariais** no menu de navegação à esquerda do Azure Active Directory.
    - Selecione **Todos os Aplicativos** para exibir uma lista de todos os seus aplicativos. Se você não vir o aplicativo que você deseja exibir aqui,  use o controle  de filtro na parte superior da lista todos os aplicativos e de definir a opção Mostrar para todos **os aplicativos**. 
    - Selecione o aplicativo que você deseja configurar para o single sign-on.
    - Depois que o aplicativo carregar, **selecione Logom único** no menu de navegação à esquerda do aplicativo.
    - Selecione **o SSO baseado em SAML.**
5. Com base no erro, para saber mais sobre as etapas recomendadas a seguir, consulte Problemas para entrar em aplicativos configurados de login único baseado em [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Para solucionar outros problemas de assinatura do usuário, consulte as seguintes diretrizes:
    - [Protocolo SAML Sign-On único](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Como solucionar erros de login usando relatórios do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Prompt de consentimento inesperado](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Erro de consentimento do usuário](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemas para entrar nos Meus Aplicativos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Erro na página de login do aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problema ao entrar em um aplicativo da Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
