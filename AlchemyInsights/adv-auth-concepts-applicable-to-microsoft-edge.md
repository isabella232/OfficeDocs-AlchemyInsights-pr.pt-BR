---
title: Conceitos de autenticação avançada aplicáveis ao Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571764"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="fb348-102">Conceitos de autenticação avançada aplicáveis ao Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="fb348-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="fb348-103">Veja a seguir os conceitos de autenticação avançada que se aplicam ao Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="fb348-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="fb348-104">**Autenticação proativa**</span><span class="sxs-lookup"><span data-stu-id="fb348-104">**Proactive Authentication**</span></span>

<span data-ttu-id="fb348-105">Quando você habilita a política [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , o Microsoft Edge tenta autenticar proativamente usuários conectados através dos serviços da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fb348-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="fb348-106">Em intervalos regulares, ele usará um serviço online para verificar se há um manifesto atualizado que contenha a configuração de controle de autenticação proativa.</span><span class="sxs-lookup"><span data-stu-id="fb348-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="fb348-107">Benefícios: a autenticação pró-ativa habilita a autenticação para os principais serviços, como a página de nova guia do Office.</span><span class="sxs-lookup"><span data-stu-id="fb348-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="fb348-108">Além disso, se o Bing for usado como o mecanismo de pesquisa, a autenticação pró-ativa melhorará o desempenho da barra de endereços e ajudará a gerar resultados de pesquisa personalizados para as necessidades de sua empresa.</span><span class="sxs-lookup"><span data-stu-id="fb348-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="fb348-109">**Windows Hello CredUI para autenticação NTLM**</span><span class="sxs-lookup"><span data-stu-id="fb348-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="fb348-110">Se o logon único (SSO) não estiver disponível quando um site tentar entrar no usuário por meio do mecanismo NTLM ou Negotiate, este recurso permitirá que o usuário Compartilhe as credenciais do sistema operacional com o site e satisfaça o desafio de autenticação usando a IU de credenciais do Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="fb348-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="fb348-111">Esse fluxo de logon aparecerá apenas no Windows 10 e apenas para usuários que não obtêm SSO durante um Challenge NTLM ou negociar.</span><span class="sxs-lookup"><span data-stu-id="fb348-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="fb348-112">**Usar senhas salvas para entrar automaticamente**</span><span class="sxs-lookup"><span data-stu-id="fb348-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="fb348-113">Os usuários que salvam senhas no Microsoft Edge podem habilitar o logon automático para sites onde foram salvas credenciais.</span><span class="sxs-lookup"><span data-stu-id="fb348-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="fb348-114">Os usuários podem ativar ou desativar esse recurso no edge://settings/passwords, e você pode configurá-lo nas políticas do [Gerenciador de senhas](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="fb348-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
