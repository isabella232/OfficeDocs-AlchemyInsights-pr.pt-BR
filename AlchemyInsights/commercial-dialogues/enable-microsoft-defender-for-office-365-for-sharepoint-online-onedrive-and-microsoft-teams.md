---
title: Habilitar o Microsoft Defender para Office 365 para SharePoint Online, OneDrive e Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735259"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="96552-102">Habilitar o Microsoft Defender para Office 365 para SharePoint Online, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="96552-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="96552-103">Usando suas credenciais de administrador global ou administrador de segurança, faça logoff no Centro de Conformidade e Segurança do [Office 365.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="96552-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="96552-104">Selecione **Gerenciamento de ameaças** no painel esquerdo e selecione **Anexos seguros** de  >  [política.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="96552-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="96552-105">Selecione **Ativar o Microsoft Defender para Office 365 para SharePoint, OneDrive** e Microsoft Teams e selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="96552-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="96552-106">Como administrador global ou administrador do SharePoint Online, execute o seguinte cmdlet do PowerShell com o parâmetro **DisallowInfectedFileDownload** definido como *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="96552-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="96552-107">Configurar alertas para arquivos detectados</span><span class="sxs-lookup"><span data-stu-id="96552-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="96552-108">Para obter mais informações, consulte [Microsoft Defender for Office 365 for SharePoint, OneDrive e Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="96552-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
