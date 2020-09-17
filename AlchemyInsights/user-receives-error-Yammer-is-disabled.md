---
title: O usuário recebe o erro AADSTS7000112 o Yammer está desabilitado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796636"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="b9d6d-102">O usuário recebe o erro AADSTS7000112 o Yammer está desabilitado</span><span class="sxs-lookup"><span data-stu-id="b9d6d-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="b9d6d-103">Se você receber a mensagem de erro "AADSTS7000112: aplicativo '00000005-0000-0ff1-ce00-000000000000' "(Yammer) está desabilitado", há um problema com a entidade de serviço no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="b9d6d-104">Um administrador pode ter desabilitado a entidade de serviço para bloquear o acesso ao Yammer.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="b9d6d-105">Desabilitar a entidade de serviço não é recomendável e pode causar problemas adicionais.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="b9d6d-106">Para obter mais informações sobre a abordagem adequada para bloquear o acesso do usuário ao Yammer, confira [Desativar o acesso ao Yammer para usuários do Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="b9d6d-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="b9d6d-107">Para corrigir esse problema no portal do Azure e restaurar o acesso do usuário ao Yammer:</span><span class="sxs-lookup"><span data-stu-id="b9d6d-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="b9d6d-108">Abra a página do Azure Active Directory e selecione **Aplicativos corporativos** em **Gerenciar** no painel de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="b9d6d-109">Digite **Office 365 Yammer** na caixa de pesquisa e selecione o nome do aplicativo para abrir as configurações.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="b9d6d-110">Selecione **Propriedades** em **Gerenciar** no painel de navegação à esquerda.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="b9d6d-111">Defina o valor da **Habilitada para que os usuários entrem?** para**Sim**e selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="b9d6d-112">Entre no Yammer novamente.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-112">Sign in to Yammer again.</span></span> <span data-ttu-id="b9d6d-113">Talvez seja necessário limpar os cookies.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-113">You might need to clear cookies.</span></span>

<span data-ttu-id="b9d6d-114">Como alternativa, execute os comandos do PowerShell para definir o valor.</span><span class="sxs-lookup"><span data-stu-id="b9d6d-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="b9d6d-115">Para saber mais, confira o artigo [Erro "Infelizmente, você está com problemas para entrar" quando você clica no bloco do Yammer no Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="b9d6d-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 