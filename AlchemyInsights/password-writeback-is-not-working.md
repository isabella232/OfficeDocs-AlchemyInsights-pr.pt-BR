---
title: O Write-back de senha não está funcionando
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232649"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="f3212-102">O Write-back de senha não está funcionando</span><span class="sxs-lookup"><span data-stu-id="f3212-102">Password Writeback is not working</span></span>

<span data-ttu-id="f3212-103">**Estou com problemas para configurar o write-back de senha**</span><span class="sxs-lookup"><span data-stu-id="f3212-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="f3212-104">O write-back de senha é um recurso premium.</span><span class="sxs-lookup"><span data-stu-id="f3212-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="f3212-105">Certifique-se de que você compreende os requisitos de licenciamento:</span><span class="sxs-lookup"><span data-stu-id="f3212-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="f3212-106">Você deve ter pelo menos uma licença atribuída em sua organização</span><span class="sxs-lookup"><span data-stu-id="f3212-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="f3212-107">**Usuários somente na** nuvem - Qualquer SKU paga do Office 365 (O365) ou Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="f3212-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="f3212-108">Usuários na nuvem **e/ou** locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="f3212-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="f3212-109">Para saber mais sobre os requisitos de licenciamento, confira Requisitos de licenciamento para redefinição de senha de [autoatendado do Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="f3212-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="f3212-110">Você tem pelo menos uma conta de administrador e uma conta de usuário de teste com uma das licenças apropriadas.</span><span class="sxs-lookup"><span data-stu-id="f3212-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="f3212-111">Você deve conectar o Azure AD Connect ao Emulador controlador de domínio primário para que o write-back de senha funcione.</span><span class="sxs-lookup"><span data-stu-id="f3212-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="f3212-112">Você pode configurar o Azure AD Connect para usar  um Controlador de Domínio Primário clicando com o botão direito do mouse nas propriedades do conector de sincronização do Active Directory e selecionando configurar partições **de diretório.**</span><span class="sxs-lookup"><span data-stu-id="f3212-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="f3212-113">A partir daí, procure a **seção** de configurações de conexão do controlador de domínio e marque a caixa intitulo apenas para **usar controladores de domínio preferenciais.**</span><span class="sxs-lookup"><span data-stu-id="f3212-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="f3212-114">Se o DC preferencial não for um emulador PDC, o Azure AD Connect ainda chegará ao PDC para write-back de senha.</span><span class="sxs-lookup"><span data-stu-id="f3212-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="f3212-115">A redefinição de senha foi configurada e habilitada em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="f3212-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="f3212-116">Para saber mais, confira [Habilitar os usuários a redefinir suas senhas do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="f3212-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="f3212-117">Certifique-se de que a conta de administrador que está sendo usada para habilitar o Write-back de Senha seja uma conta de administrador de nuvem (criada no Azure AD e não no AD local)</span><span class="sxs-lookup"><span data-stu-id="f3212-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="f3212-118">Você tem uma implantação local do AD de floresta única ou com várias florestas executando o Windows Server 2008 R2, o Windows Server 2012 ou o Windows Server 2012 R2 com os service packs mais recentes instalados</span><span class="sxs-lookup"><span data-stu-id="f3212-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="f3212-119">Você tem a ferramenta Azure AD Connect instalada e preparou seu ambiente do AD para sincronização com a nuvem.</span><span class="sxs-lookup"><span data-stu-id="f3212-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="f3212-120">Antes de testar o write-back de senha, primeiro certifique-se de concluir uma importação completa e uma sincronização completa do AD e do Azure AD no Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f3212-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="f3212-121">Para saber mais, veja como fazer uma sincronização completa e [a importação completa no Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="f3212-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="f3212-122">**Estou tendo um problema com a conectividade de write-back de senha**</span><span class="sxs-lookup"><span data-stu-id="f3212-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="f3212-123">Baixar e habilitar a versão mais recente do [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="f3212-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="f3212-124">Configuração de firewall: a ferramenta Azure AD Connect (1.1.443 e superior) precisará de acesso **HTTPS** de saída para:</span><span class="sxs-lookup"><span data-stu-id="f3212-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="f3212-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f3212-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="f3212-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="f3212-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="f3212-127">Permitir que conexões ociosas persistam por pelo menos 2 a 3 minutos</span><span class="sxs-lookup"><span data-stu-id="f3212-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="f3212-128">**Ainda estou tendo problemas com o write-back de senha**</span><span class="sxs-lookup"><span data-stu-id="f3212-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="f3212-129">Se você ainda estiver com dificuldades, tente desabilitar e reabilgrafar o serviço de write-back de senha na ferramenta Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f3212-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="f3212-130">Para saber mais, veja como desabilitar [e reabilitar o write-back de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="f3212-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
