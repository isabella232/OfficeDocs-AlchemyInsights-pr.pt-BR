---
title: 932 atualizando AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506071"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="4741a-102">Atualizar Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="4741a-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="4741a-103">Por padrão, a atualização automática está habilitada para o Azure AD Connect, o que ajuda a garantir que você esteja executando a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="4741a-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="4741a-104">Para verificar as configurações de atualização automática, use o cmdlet **Get-ADSyncAutoUpgrade** no PowerShell do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4741a-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="4741a-105">O cmdlet retornará um dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="4741a-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="4741a-106">**Habilitado**: a atualização automática está habilitada.</span><span class="sxs-lookup"><span data-stu-id="4741a-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="4741a-107">**Disabled**: a atualização automática está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="4741a-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="4741a-108">**Suspenso**: o sistema não está mais qualificado para receber atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="4741a-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="4741a-109">Você não pode configurar esse valor; é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="4741a-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="4741a-110">Para obter mais informações, consulte [atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="4741a-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="4741a-111">Para baixar a versão mais recente do Azure AD Connect, acesse [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="4741a-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
