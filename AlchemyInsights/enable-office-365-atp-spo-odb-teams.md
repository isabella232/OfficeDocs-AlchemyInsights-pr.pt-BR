---
title: Habilitar o Office 365 ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506906"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1a436-102">Habilitar a proteção avançada contra ameaças do Office 365 para o SharePoint Online, o OneDrive e o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1a436-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="1a436-103">Acesse https://protection.office.com e entre.</span><span class="sxs-lookup"><span data-stu-id="1a436-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="1a436-104">Escolha **Threat management**  >  **Policy**  >  **anexos seguros**da política de gerenciamento de ameaças.</span><span class="sxs-lookup"><span data-stu-id="1a436-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="1a436-105">Selecione **Ativar ATP para SharePoint, onedrive e Microsoft Teams**e clique em **salvar**.</span><span class="sxs-lookup"><span data-stu-id="1a436-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="1a436-106">Recomenda Como administrador global ou administrador do SharePoint Online, execute o cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido como *true*.</span><span class="sxs-lookup"><span data-stu-id="1a436-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="1a436-107">Recomenda [Configurar alertas](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para arquivos detectados.</span><span class="sxs-lookup"><span data-stu-id="1a436-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="1a436-108">A ATP deixará a verificação de todos os arquivos no SharePoint Online, no OneDrive ou no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1a436-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="1a436-109">Os arquivos são verificados de forma assíncrona por meio de um processo que usa eventos de atividade de compartilhamento e convidados, juntamente com heurística inteligente e sinais de ameaça para identificar arquivos mal-intencionados.</span><span class="sxs-lookup"><span data-stu-id="1a436-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="1a436-110">Consulte [ATP para SharePoint, onedrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="1a436-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>