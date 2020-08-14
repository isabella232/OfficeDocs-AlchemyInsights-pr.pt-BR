---
title: Alterar canais de atualização de Aplicativos do Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: fb69bce40ab56b162c715af6a0647c8219c5564f
ms.sourcegitcommit: dab885f2cb99057e959fb9be334f5a3a26a64058
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2020
ms.locfileid: "46665450"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="13df2-102">Alterar canais de atualização de Aplicativos do Office</span><span class="sxs-lookup"><span data-stu-id="13df2-102">Change update channels for Office apps</span></span>

<span data-ttu-id="13df2-103">Para novas instalações do Office, use as Configurações de Download de Software do Office para escolher o canal de atualização e, em seguida, instale (ou reinstale) os aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="13df2-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="13df2-104">Para saber mais, veja [Gerenciar as Configurações de Download de Software no Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span><span class="sxs-lookup"><span data-stu-id="13df2-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="13df2-105">**Observação** o canal de atualização selecionado usando as Configurações de Download de Software do Office se aplica a todos os usuários executando novas instalações usando o portal do O365.</span><span class="sxs-lookup"><span data-stu-id="13df2-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="13df2-106">Para saber mais informações, confira [Baixar e instalar ou reinstalar o Microsoft 365 ou o Office 2019 em PC ou Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span><span class="sxs-lookup"><span data-stu-id="13df2-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="13df2-107">Para instalações existentes do Office, use a Ferramenta de Implantação do Office (ODT) para mudar para outro um canal de atualização:</span><span class="sxs-lookup"><span data-stu-id="13df2-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="13df2-108">Baixe a versão mais recente da Ferramenta de Implantação do Office (setup.exe) no [Centro de Download da Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="13df2-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="13df2-109">Identifique o nome do canal para o qual você deseja mudar.</span><span class="sxs-lookup"><span data-stu-id="13df2-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="13df2-110">Para saber mais informações, veja [Opções de configuração da Ferramenta de Implantação do Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span><span class="sxs-lookup"><span data-stu-id="13df2-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="13df2-111">Crie um arquivo XML de configuração especificando o nome do canal apropriado, por exemplo, update.xml.</span><span class="sxs-lookup"><span data-stu-id="13df2-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  
    `<Configuration> 
    <Updates **Channel="Monthly"** />  
    </Configuration>`
4. <span data-ttu-id="13df2-112">Em um prompt de comando elevado, alterne para o local da pasta do setup.exe e execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="13df2-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="13df2-113">a.</span><span class="sxs-lookup"><span data-stu-id="13df2-113">a.</span></span> <span data-ttu-id="13df2-114">setup.exe /configure update.xml</span><span class="sxs-lookup"><span data-stu-id="13df2-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="13df2-115">Inicie um aplicativo do Office (como o Excel) e, em seguida, selecione **Arquivo** > **Conta**.</span><span class="sxs-lookup"><span data-stu-id="13df2-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="13df2-116">Na seção Informações do Produto, selecione **Opções de Atualização** > **Atualizar Agora**.</span><span class="sxs-lookup"><span data-stu-id="13df2-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="13df2-117">Para saber mais, veja [Como alternar canais de atualização de aplicativos existentes do Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span><span class="sxs-lookup"><span data-stu-id="13df2-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="13df2-118">Para alternar os canais de atualização de um grupo de usuários selecionado ou usando o Configuration Manager (SCCM), defina a configuração do Canal de Atualização usando o GPO.</span><span class="sxs-lookup"><span data-stu-id="13df2-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="13df2-119">Para obter mais informações, confira [Visão geral dos canais de atualização do Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span><span class="sxs-lookup"><span data-stu-id="13df2-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="13df2-120">Para obter detalhes, confira [Como gerenciar canais do Office 365 ProPlus para profissionais de TI](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) e [Gerenciar atualizações do Microsoft 365 Apps com o Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="13df2-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>