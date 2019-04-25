---
title: 932 atualizando AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389644"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="b1eb4-102">Atualizar Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="b1eb4-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="b1eb4-103">Por padrão, a atualização automática está habilitada para o Azure AD Connect, o que ajuda a garantir que você esteja executando a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="b1eb4-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="b1eb4-104">Para verificar as configurações de atualização automática, use o cmdlet **Get-ADSyncAutoUpgrade** no PowerShell do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1eb4-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="b1eb4-105">O cmdlet retornará um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="b1eb4-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="b1eb4-106">**Habilitado**: a atualização automática está habilitada.</span><span class="sxs-lookup"><span data-stu-id="b1eb4-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="b1eb4-107">**Disabled**: a atualização automática está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="b1eb4-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="b1eb4-108">**Suspenso**: o sistema não está mais qualificado para receber atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="b1eb4-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="b1eb4-109">Você não pode configurar esse valor; é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="b1eb4-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="b1eb4-110">Para obter mais informações, consulte [atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="b1eb4-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="b1eb4-111">Para baixar a versão mais recente do Azure AD Connect, acesse [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="b1eb4-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
