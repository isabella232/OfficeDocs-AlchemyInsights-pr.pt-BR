---
title: Conceitos avançados de autenticação aplicáveis ao Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398538"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="33607-102">Conceitos avançados de autenticação aplicáveis ao Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="33607-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="33607-103">A seguir estão os conceitos avançados de autenticação aplicáveis ao Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="33607-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="33607-104">**Autenticação Proativa**</span><span class="sxs-lookup"><span data-stu-id="33607-104">**Proactive Authentication**</span></span>

<span data-ttu-id="33607-105">Quando você habilitar [a política ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) o Microsoft Edge tentará autenticar proativamente os usuários de entrada por meio dos serviços Microsoft.</span><span class="sxs-lookup"><span data-stu-id="33607-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="33607-106">Em intervalos regulares, ele usará um serviço online para verificar se há um manifesto atualizado que contém a configuração que rege a Autenticação Proativa.</span><span class="sxs-lookup"><span data-stu-id="33607-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="33607-107">Benefícios: a Autenticação Proativa habilita a autenticação para serviços principais, como a Página nova guia do Office.</span><span class="sxs-lookup"><span data-stu-id="33607-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="33607-108">Além disso, se o Bing for usado como mecanismo de pesquisa, a Autenticação Proativa melhora o desempenho da barra de endereços e ajuda a gerar resultados de pesquisa personalizados para as necessidades da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="33607-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="33607-109">**Windows Hello CredUI para autenticação NTLM**</span><span class="sxs-lookup"><span data-stu-id="33607-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="33607-110">Se o SSO (login único) não estiver disponível quando um site tentar entrar no usuário por meio do mecanismo NTLM ou Negociar, esse recurso permitirá que o usuário compartilhe as credenciais do sistema operacional com o site e atenda ao desafio de autenticação usando a interface do usuário do Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="33607-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="33607-111">Esse fluxo de login aparecerá somente no Windows 10 e somente para usuários que não receberem SSO durante um NTLM ou um desafio Negociar.</span><span class="sxs-lookup"><span data-stu-id="33607-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="33607-112">**Usar senhas salvas para entrar automaticamente**</span><span class="sxs-lookup"><span data-stu-id="33607-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="33607-113">Os usuários que salvam senhas no Microsoft Edge podem habilitar o login automático em sites onde salvaram credenciais.</span><span class="sxs-lookup"><span data-stu-id="33607-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="33607-114">Os usuários podem ativar ou desativar esse recurso edge://settings/passwords e você pode configurá-lo nas políticas de gerenciador [de](https://go.microsoft.com/fwlink/?linkid=2134622) senhas.</span><span class="sxs-lookup"><span data-stu-id="33607-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
