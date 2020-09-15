---
title: ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715549"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="23a2a-102">ATP para SharePoint, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="23a2a-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="23a2a-103">Siga estas etapas para habilitar a proteção avançada contra ameaças:</span><span class="sxs-lookup"><span data-stu-id="23a2a-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="23a2a-104">Acesse [https://protection.office.com](https://protection.office.com) e entre com uma conta de administrador global ou administrador de segurança.</span><span class="sxs-lookup"><span data-stu-id="23a2a-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="23a2a-105">No painel de navegação esquerdo em **Gerenciamento de ameaças**, **Policy** escolha \> **anexos seguros**da política.</span><span class="sxs-lookup"><span data-stu-id="23a2a-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="23a2a-106">Selecione **Ativar ATP para SharePoint, onedrive e Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="23a2a-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="23a2a-107">[Crie uma política de alerta de atividade](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) para receber notificações quando detectarmos arquivos mal-intencionados.</span><span class="sxs-lookup"><span data-stu-id="23a2a-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="23a2a-108">Para obter instruções completas, consulte este [tópico](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="23a2a-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="23a2a-109">**Observação**: por design, a ATP não examina todos os arquivos no SharePoint Online, no onedrive for Business ou no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="23a2a-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="23a2a-110">Os arquivos são verificados de forma assíncrona por um processo que usa atividade de compartilhamento, atividade de convidado e sinais de ameaça para identificar arquivos mal-intencionados.</span><span class="sxs-lookup"><span data-stu-id="23a2a-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="23a2a-111">Para obter mais informações, consulte este [tópico](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="23a2a-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
