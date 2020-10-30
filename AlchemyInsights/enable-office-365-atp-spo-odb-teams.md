---
title: Habilitar o Office 365 ATP para SharePoint, OneDrive e Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801035"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="9a215-102">Habilitar o Microsoft defender para Office 365 para SharePoint Online, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9a215-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="9a215-103">Acesse https://protection.office.com e entre.</span><span class="sxs-lookup"><span data-stu-id="9a215-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="9a215-104">Escolha **Threat management**  >  **Policy**  >  **anexos seguros** da política de gerenciamento de ameaças.</span><span class="sxs-lookup"><span data-stu-id="9a215-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="9a215-105">Selecione **Ativar ATP para SharePoint, onedrive e Microsoft Teams** e clique em **salvar** .</span><span class="sxs-lookup"><span data-stu-id="9a215-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="9a215-106">Recomenda Como administrador global ou administrador do SharePoint Online, execute o cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) com o parâmetro **DisallowInfectedFileDownload** definido como *true* .</span><span class="sxs-lookup"><span data-stu-id="9a215-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="9a215-107">Recomenda [Configurar alertas](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) para arquivos detectados.</span><span class="sxs-lookup"><span data-stu-id="9a215-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="9a215-108">A ATP deixará a verificação de todos os arquivos no SharePoint Online, no OneDrive ou no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9a215-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="9a215-109">Os arquivos são verificados de forma assíncrona por meio de um processo que usa eventos de atividade de compartilhamento e convidados, juntamente com heurística inteligente e sinais de ameaça para identificar arquivos mal-intencionados.</span><span class="sxs-lookup"><span data-stu-id="9a215-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="9a215-110">Consulte [ATP para SharePoint, onedrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="9a215-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>