---
title: Corrigir problemas de entrega de emails em pastas públicas habilitadas para email
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387693"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="cd083-102">Corrigir problemas de entrega de emails em pastas públicas habilitadas para email</span><span class="sxs-lookup"><span data-stu-id="cd083-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="cd083-103">Se os remetentes externos não podem enviar mensagens para suas pastas públicas habilitadas para email, e os remetentes receberem o erro: **não foi possível encontrar (550 5.4.1)**, verifique se o domínio de email da pasta pública está configurado como um domínio de retransmissão interno em vez de um domínio autoritativo:</span><span class="sxs-lookup"><span data-stu-id="cd083-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="cd083-104">Abra o [centro de administração do Exchange (Eat)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="cd083-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="cd083-105">Vá para \*\*\*\* \> **domínios aceitos**do fluxo de emails, selecione o domínio aceito e clique em **Editar**.</span><span class="sxs-lookup"><span data-stu-id="cd083-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="cd083-106">Na página de propriedades que será aberta, se o tipo de domínio estiver definido como **autoritativo**, altere o valor para **retransmissão interna** e clique em **salvar**.</span><span class="sxs-lookup"><span data-stu-id="cd083-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="cd083-107">Se os remetentes externos receberem o erro **que você não tem permissão (550 5.7.13)**, execute o seguinte comando no [PowerShell do Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver as permissões para usuários anônimos na pasta pública:</span><span class="sxs-lookup"><span data-stu-id="cd083-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="cd083-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Por exemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="cd083-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="cd083-109">Para permitir que usuários externos enviem email para esta pasta pública, adicione o direito de acesso CreateItems ao usuário anônimo.</span><span class="sxs-lookup"><span data-stu-id="cd083-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="cd083-110">Por exemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="cd083-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
