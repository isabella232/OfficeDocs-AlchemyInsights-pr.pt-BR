---
title: Problemas com links e URLs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950657"
---
# <a name="issues-with-links-and-urls"></a>Problemas com links e URLs

URLs de resposta/URI de redirecionamento (ambas as expressões são intercambiáveis) são as URLs usadas pela plataforma de identidade da Microsoft para retornar os tokens solicitados pelo aplicativo. Para obter informações sobre essas URLs, veja os seguintes artigos:

- [Fluxos de autenticação e cenários de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – Informações sobre as URIs de redirecionamento na página de **Registro do app** para cada cenário.
- [Restrições e limitações de URLs de resposta/URI de redirecionamento](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Não sei como registrar a URL de resposta/URI de redirecionamento correta para o meu aplicativo**

Ao entrar com o aplicativo que você está desenvolvendo, se a caixa de diálogo de entrada exibir **AADSTS50011: A url de resposta especificada na solicitação não corresponde às urls de resposta configuradas para o aplicativo <your app ID>**, você precisará adicionar ao registro do aplicativo, a URI de redirecionamento que seu código usou na solicitação de token para a plataforma de identidade da Microsoft.

Para adicionar uma URL de resposta, vá para a guia **Autenticação** na página de **registro do aplicativo** no portal do Azure e adicione uma entrada na seção **URIs de redirecionamento**. As URIs de redirecionamento são digitadas (Web ou celular/área de trabalho). O valor que você precisa inserir depende do tipo de aplicativo que você está criando, conforme descrito abaixo:

- Para aplicativos de página única e apps Web, a URL de resposta é uma URL do seu aplicativo. Veja [Registro do aplicativo de página única](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ou [Registrar um app da Web usando o portal do Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Para apps da área de trabalho, o valor que você precisa escolher depende de:
    - a plataforma (MacOS é diferente do Windows ou Linux)
    - a maneira como você adquire o token (interativamente, com fluxo de código do dispositivo, com a IWA [Autenticação integrada do Windows] ou com nome de usuário/senha).
    Para obter detalhes, veja [Apps da área de trabalho – Registro de app – URI de redirecionamento](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Para aplicativos móveis, a URI de redirecionamento depende de:
    - a plataforma (iOS/Android/UWP)
    - as informações usadas para criar seu app, como a ID do pacote no iOS, o nome do pacote e o hash de assinatura no android; o registro de app do portal do Azure ajudará você. Para obter detalhes, veja [Configuração da plataforma e URIs de redirecionamento](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> As APIs da Web e algumas das formas silenciosas de adquirir tokens (IWA e nome de usuário/senha) não exigem uma URI de redirecionamento.

**Já implantei meu aplicativo Web e quando o testei, recebi uma mensagem de incompatibilidade da url de resposta**

Adicione URIs de redirecionamento em todos os locais que você está implantando seu aplicativo Web. Para obter mais informações, veja [Registrar um aplicativo Web usando o portal do Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Adicione a URI de redirecionamento em um local imediatamente após a implantação do aplicativo nesse local.

**Não consigo registrar URLs de resposta suficientes**

Você é um ISV, e tem uma ou várias URIs de redirecionamento para cada cliente. Você quer migrar de ADAL/Azure AD v1.0 para MSAL/a plataforma de identidade da Microsoft, e você atinge o [número máximo de URIs de redirecionamento](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Para resolver isso, [adicione URIs de redirecionamento às entidades de serviço](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) que correspondem a cada um de seus clientes.
