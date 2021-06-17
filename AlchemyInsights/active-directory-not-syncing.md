---
title: Não sincronização do Active Directory
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930963"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="3a4f5-102">Não sincronização do Active Directory</span><span class="sxs-lookup"><span data-stu-id="3a4f5-102">Active Directory not syncing</span></span>

<span data-ttu-id="3a4f5-103">Se você estiver recebendo erros de sincronização, como "nenhuma sincronização recente", ou observe que o status de sincronização de diretório no portal de administração do Office diz: "A última sincronização foi há mais de 3 dias", pode ser que o AADConnect tenha configurações incorretas ou permissões insuficientes para executar uma sincronização.</span><span class="sxs-lookup"><span data-stu-id="3a4f5-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="3a4f5-104">Reinstalar o AADConnect usando configurações expressas pode resolver o problema rapidamente:</span><span class="sxs-lookup"><span data-stu-id="3a4f5-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="3a4f5-105">[Baixe a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="3a4f5-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="3a4f5-106">[Siga as instruções para instalação expressa](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="3a4f5-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="3a4f5-107">O Azure AD Connect deve ser instalado no Windows Server 2012 ou versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="3a4f5-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="3a4f5-108">Esse servidor deve ser integrado ao domínio e pode ser um controlador de domínio ou um servidor membro.</span><span class="sxs-lookup"><span data-stu-id="3a4f5-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="3a4f5-109">Para uma lista completa de requisitos e pré-requisitos do Azure AD Conexão, revise Os pré-requisitos do [Azure AD Conexão](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="3a4f5-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="3a4f5-110">Para mais informações sobre contas de serviço do AADConnect, confira [Azure AD Connect: Contas e permissões](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="3a4f5-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
