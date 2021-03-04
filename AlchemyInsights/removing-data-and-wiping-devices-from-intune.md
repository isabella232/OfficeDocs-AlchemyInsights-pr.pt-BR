---
title: Removendo dados e limpando dispositivos do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416301"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="66c32-102">Removendo dados e limpando dispositivos do Intune</span><span class="sxs-lookup"><span data-stu-id="66c32-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="66c32-103">As ações remotas de Apagamento do Dispositivo e Desativação de Dispositivo podem ser usadas para remover dados da empresa gerenciados pelo Intune ou para executar uma redefinição de fábrica e restaurar o dispositivo com as configurações padrão.</span><span class="sxs-lookup"><span data-stu-id="66c32-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="66c32-104">Entre no Gerenciamento de Dispositivo do Microsoft 365, e vá para **Dispositivos** > **Todos Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="66c32-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="66c32-105">Selecione o dispositivo que deseja apagar.</span><span class="sxs-lookup"><span data-stu-id="66c32-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="66c32-106">Selecione o tipo de apagamento remoto que deseja executar.</span><span class="sxs-lookup"><span data-stu-id="66c32-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="66c32-107">A desativação exclui somente as informações organizacionais, enquanto as exclusões completas restauram o dispositivo para suas configurações de fábrica.</span><span class="sxs-lookup"><span data-stu-id="66c32-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="66c32-108">Selecione **Sim** para confirmar.</span><span class="sxs-lookup"><span data-stu-id="66c32-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="66c32-109">Até que a limpeza seja concluída, o status de ação do dispositivo é mostrado como *Retire Pending*.</span><span class="sxs-lookup"><span data-stu-id="66c32-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="66c32-110">Após a conclusão da ação, você não verá mais o dispositivo móvel na lista de dispositivos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="66c32-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="66c32-111">Dados da empresa não podem ser removidos dos dispositivos UNIDOS ao Microsoft Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="66c32-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="66c32-112">Para obter detalhes completos sobre o efeito das ações Retirar e Limpar, incluindo o que é retido e o que é excluído, consulte a seguinte documentação:</span><span class="sxs-lookup"><span data-stu-id="66c32-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="66c32-113">[Remova dispositivos limpando, retirando ou cancelando a inscrição manualmente](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="66c32-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="66c32-114">Como limpar apenas dados corporativos de aplicativos gerenciados pelo Intune</span><span class="sxs-lookup"><span data-stu-id="66c32-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="66c32-115">[Apague todos os dados de um dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="66c32-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>