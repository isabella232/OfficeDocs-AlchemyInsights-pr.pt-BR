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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701271"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="44fb5-102">Removendo dados e limpando dispositivos do Intune</span><span class="sxs-lookup"><span data-stu-id="44fb5-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="44fb5-103">As ações remotas de Apagamento do Dispositivo e Desativação de Dispositivo podem ser usadas para remover dados da empresa gerenciados pelo Intune ou para executar uma redefinição de fábrica e restaurar o dispositivo com as configurações padrão.</span><span class="sxs-lookup"><span data-stu-id="44fb5-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="44fb5-104">Entre no Gerenciamento de Dispositivo do Microsoft 365, e vá para **Dispositivos** > **Todos Dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="44fb5-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="44fb5-105">Selecione o dispositivo que deseja apagar.</span><span class="sxs-lookup"><span data-stu-id="44fb5-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="44fb5-106">Selecione o tipo de apagamento remoto que deseja executar.</span><span class="sxs-lookup"><span data-stu-id="44fb5-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="44fb5-107">A desativação exclui somente as informações organizacionais, enquanto as exclusões completas restauram o dispositivo para suas configurações de fábrica.</span><span class="sxs-lookup"><span data-stu-id="44fb5-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="44fb5-108">Selecione **Sim** para confirmar.</span><span class="sxs-lookup"><span data-stu-id="44fb5-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="44fb5-109">Até que o apagamento seja concluído, o status da ação do Dispositivo é mostrado como Desativação Pendente.</span><span class="sxs-lookup"><span data-stu-id="44fb5-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="44fb5-110">Após a conclusão da ação, você não verá mais o dispositivo móvel na lista de dispositivos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="44fb5-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="44fb5-111">**Observação** Dados da empresa não podem ser removidos de dispositivos ASSOCIADOS ao Azure AD.</span><span class="sxs-lookup"><span data-stu-id="44fb5-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="44fb5-112">Para detalhes completos sobre o efeito das ações de Desativar e Apagar, incluindo o que é mantido e o que é excluído, confira [Remover dispositivos usando apagar, desativar ou manualmente cancelar o registro do dispositivo](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="44fb5-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="44fb5-113">Para apagar todos os dados de um dispositivo macOS, confira [Apagar todos os dados de um dispositivo macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="44fb5-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>