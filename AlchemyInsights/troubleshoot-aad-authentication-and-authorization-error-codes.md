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
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897467"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="99e83-102">Solucionar problemas de Autenticação do Microsoft Azure AD e códigos de erro de autorização (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="99e83-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="99e83-103">Para resolver os códigos de erro de autorização e autenticação AADAD (AADSTS), execute as seguintes etapas recomendadas:</span><span class="sxs-lookup"><span data-stu-id="99e83-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="99e83-104">**Manipulando códigos de erro em seu aplicativo**</span><span class="sxs-lookup"><span data-stu-id="99e83-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="99e83-105">A **especificação OAuth2.0**, https://tools.ietf.org/html/rfc6749#section-5.2, fornece orientação sobre como lidar com erros durante a autenticação usando a parte error da resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="99e83-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="99e83-106">**error**: uma cadeia de caracteres de código de erro que pode ser usada para classificar os tipos de erros que ocorrem e deve ser usada para reação a erros.</span><span class="sxs-lookup"><span data-stu-id="99e83-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="99e83-107">O campo **error** tem vários valores possíveis: revise os links de documentação do protocolo e as especificações do OAuth 2.0 para obter mais informações sobre erros específicos e como reagir a eles.</span><span class="sxs-lookup"><span data-stu-id="99e83-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="99e83-108">Aqui está um exemplo de resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="99e83-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="99e83-109">**Procurar informações de código de erro atual**</span><span class="sxs-lookup"><span data-stu-id="99e83-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="99e83-110">Os códigos de erro e as mensagens estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99e83-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="99e83-111">Para obter as informações mais atuais, consulte a página https://login.microsoftonline.com/error para encontrar descrições de erro AADSTS, correções e algumas soluções alternativas sugeridas.</span><span class="sxs-lookup"><span data-stu-id="99e83-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="99e83-112">Você também pode pesquisar e solucionar problemas de códigos de erro [ de erro AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listados no artigo [Autenticação do Microsoft Azure AD e códigos de erro de autorização](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="99e83-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="99e83-113">**Obter Ajuda**</span><span class="sxs-lookup"><span data-stu-id="99e83-113">**Get Help**</span></span>

- <span data-ttu-id="99e83-114">[Opções de ajuda e suporte para desenvolvedores](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) : se você precisar de uma resposta para uma pergunta ou ajuda para resolver um problema não abordado em nossa documentação, talvez seja hora de falar com especialistas para pedir ajuda.</span><span class="sxs-lookup"><span data-stu-id="99e83-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="99e83-115">Este artigo fornece várias sugestões para obter respostas para suas perguntas à medida que você desenvolve aplicativos que se integram à plataforma de identidade para desenvolvedores da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="99e83-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








