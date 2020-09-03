---
title: Controlar atualizações automáticas de Aplicativos do Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431296"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="18930-102">Controlar atualizações automáticas de Aplicativos do Office</span><span class="sxs-lookup"><span data-stu-id="18930-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="18930-103">Por padrão, atualizações de Aplicativos do Office são baixadas e aplicadas automaticamente em segundo plano, sem nenhuma intervenção do usuário.</span><span class="sxs-lookup"><span data-stu-id="18930-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="18930-104">No entanto, os administradores podem controlar como as atualizações são aplicadas usando as configurações de Atualização do Office.</span><span class="sxs-lookup"><span data-stu-id="18930-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="18930-105">As configurações de atualização permitem aos administradores habilitar ou desabilitar atualizações automáticas, mostrar ou ocultar o botão **Atualizar agora** no Office, definir prazos de atualização e muito mais.</span><span class="sxs-lookup"><span data-stu-id="18930-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="18930-106">Para obter informações detalhadas, veja:</span><span class="sxs-lookup"><span data-stu-id="18930-106">For detailed information, see:</span></span>

- [<span data-ttu-id="18930-107">Configurar definições de atualização do Office</span><span class="sxs-lookup"><span data-stu-id="18930-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="18930-108">Atualização automática do Office não está habilitada</span><span class="sxs-lookup"><span data-stu-id="18930-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="18930-109">Definir como o Office será atualizado após sua instalação</span><span class="sxs-lookup"><span data-stu-id="18930-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="18930-110">Para analisar as configurações de atualizações existentes aplicadas a um computador cliente, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="18930-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="18930-111">Abra o Editor do Registro acessando **Iniciar** > **Executar** > **regedit**.</span><span class="sxs-lookup"><span data-stu-id="18930-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="18930-112">Mude para o local a seguir e analise as configurações de Atualização do Office:</span><span class="sxs-lookup"><span data-stu-id="18930-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="18930-113">a.</span><span class="sxs-lookup"><span data-stu-id="18930-113">a.</span></span> <span data-ttu-id="18930-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="18930-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="18930-115">b.</span><span class="sxs-lookup"><span data-stu-id="18930-115">b.</span></span> <span data-ttu-id="18930-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="18930-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="18930-117">**Observação** se a chave OfficeMgmtCOM estiver definida, você poderá ver a mensagem "Atualizações são gerenciadas pelo administrador do sistema" em **Office** > **Conta** > **Atualizações do Office**.</span><span class="sxs-lookup"><span data-stu-id="18930-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="18930-118">Para saber mais, confira [Gerenciar atualizações do Microsoft 365 Apps com o Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="18930-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  