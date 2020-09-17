---
title: Não é possível entrar no Teams devido ao erro autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799948"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="f8eaf-102">Não é possível entrar no Teams devido ao erro autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="f8eaf-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="f8eaf-103">Se o SSO Contínuo estiver ativado como a autenticação do O365, talvez seja necessário adicionar a URL "autologon.microsoftazuread-sso.com" aos Sites da Intranet.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="f8eaf-104">Se ela tiver sido adicionada anteriormente aos Sites Confiáveis e o SSO Contínuo estiver em uso, ela deve ser removida dos Sites Confiáveis.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="f8eaf-105">Examine a [lista de verificação de solução de problemas de SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="f8eaf-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="f8eaf-106">Siga estas etapas para adicionar uma URL à lista de Sites da Intranet:</span><span class="sxs-lookup"><span data-stu-id="f8eaf-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="f8eaf-107">Abra o Internet Explorer clicando no botão **Iniciar**.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="f8eaf-108">Na caixa de pesquisa, digite Internet Explorer e, em seguida, na lista de resultados, clique em **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="f8eaf-109">Clique em **Ferramentas** e em **Opções da Internet**.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="f8eaf-110">Clique na guia **Segurança**.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="f8eaf-111">Agora, clique em **Sites da intranet local** e, em seguida, clique no botão **Sites** e depois no botão **Avançado**.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="f8eaf-112">Insira a URL do site e clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="f8eaf-113">Quando terminar, clique em **Fechar**.</span><span class="sxs-lookup"><span data-stu-id="f8eaf-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="f8eaf-114">Para saber mais, confira a [Documentação para a implantação do SSO Contínuo no O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inclui o processo baseado em políticas para adicionar uma URL aos sites da intranet na etapa 3).</span><span class="sxs-lookup"><span data-stu-id="f8eaf-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
