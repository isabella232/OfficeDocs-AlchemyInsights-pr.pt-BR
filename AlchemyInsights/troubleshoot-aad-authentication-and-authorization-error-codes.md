---
title: Solucionar problemas de Autenticação do Microsoft Azure AD e códigos de erro de autorização (AADSTS)
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
- "9800"
- "9005744"
ms.openlocfilehash: ac25548b0110834c877ae53be097d6b6c0f13c4091040a901abd56fb2a3cbba3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939943"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Solucionar problemas de Autenticação do Microsoft Azure AD e códigos de erro de autorização (AADSTS)

Para resolver os códigos de erro de autorização e autenticação AADAD (AADSTS), execute as seguintes etapas recomendadas:

1. **Manipulando códigos de erro em seu aplicativo**

- A **especificação OAuth2.0**, https://tools.ietf.org/html/rfc6749#section-5.2, fornece orientação sobre como lidar com erros durante a autenticação usando a parte error da resposta de erro.

    - **error**: uma cadeia de caracteres de código de erro que pode ser usada para classificar os tipos de erros que ocorrem e deve ser usada para reação a erros.
    - O campo **error** tem vários valores possíveis: revise os links de documentação do protocolo e as especificações do OAuth 2.0 para obter mais informações sobre erros específicos e como reagir a eles.

- Aqui está um exemplo de resposta de erro:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Procurar informações de código de erro atual**

- Códigos de erro e mensagens estão sujeitos a alterações. Para obter as informações mais atuais, consulte a página https://login.microsoftonline.com/error para encontrar descrições de erros, correções e algumas soluções alternativas sugeridas do AADSTS.
- Você também pode pesquisar e solucionar problemas de códigos de erro [ de erro AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listados no artigo [Autenticação do Microsoft Azure AD e códigos de erro de autorização](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Obter Ajuda**

- [Opções de ajuda e suporte para desenvolvedores](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) : se você precisar de uma resposta para uma pergunta ou ajuda para resolver um problema não abordado em nossa documentação, talvez seja hora de falar com especialistas para pedir ajuda. Este artigo fornece várias sugestões para obter respostas para suas perguntas à medida que você desenvolve aplicativos que se integram à plataforma de identidade para desenvolvedores da Microsoft.








