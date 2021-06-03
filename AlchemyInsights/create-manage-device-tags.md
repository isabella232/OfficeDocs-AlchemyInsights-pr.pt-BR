---
title: Criar e gerenciar marcas ou grupos de dispositivo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721663"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="763f1-102">Criar e gerenciar marcas ou grupos de dispositivo</span><span class="sxs-lookup"><span data-stu-id="763f1-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="763f1-103">Adicionar marcas em dispositivos para criar uma afiliação de grupo lógico.</span><span class="sxs-lookup"><span data-stu-id="763f1-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="763f1-104">As marcas de dispositivo oferecem suporte ao mapeamento correto da rede, permitindo anexar marcas diferentes para capturar contexto e habilitar a criação de lista dinâmica como parte de um incidente.</span><span class="sxs-lookup"><span data-stu-id="763f1-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="763f1-105">As marcas podem ser usadas como um filtro no modo de exibição de lista Dispositivos ou para agrupar dispositivos.</span><span class="sxs-lookup"><span data-stu-id="763f1-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="763f1-106">Para obter mais informações sobre agrupamento de dispositivos, veja [Criar e gerenciar marcas de dispositivo](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="763f1-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="763f1-107">Você pode adicionar marcas em dispositivos ao:</span><span class="sxs-lookup"><span data-stu-id="763f1-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="763f1-108">Usar o portal</span><span class="sxs-lookup"><span data-stu-id="763f1-108">Using the portal</span></span>

- <span data-ttu-id="763f1-109">Definir um valor de chave de registro</span><span class="sxs-lookup"><span data-stu-id="763f1-109">Setting a registry key value</span></span>
 
<span data-ttu-id="763f1-110">**Observação:** Pode haver latência entre o momento que uma marca for adicionada a um dispositivo e sua disponibilidade na lista de dispositivos e na página de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="763f1-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="763f1-111">Para adicionar marcas de dispositivo usando a API, veja a [API Adicionar ou remover marcas de dispositivo](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="763f1-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="763f1-112">Adicionar e gerenciar marcas de dispositivo usando o portal</span><span class="sxs-lookup"><span data-stu-id="763f1-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="763f1-113">Selecione o dispositivo o qual você deseja gerenciar as marcas.</span><span class="sxs-lookup"><span data-stu-id="763f1-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="763f1-114">Você pode selecionar ou procurar um dispositivo a partir de qualquer uma dos modos de exibição a seguir:</span><span class="sxs-lookup"><span data-stu-id="763f1-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="763f1-115">**Painel de operações de segurança** Selecione o nome do dispositivo nos Principais dispositivos com a seção de alertas ativos.</span><span class="sxs-lookup"><span data-stu-id="763f1-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="763f1-116">**Fila de alertas** - Selecione o nome do dispositivo ao lado do ícone do dispositivo na fila de alertas.</span><span class="sxs-lookup"><span data-stu-id="763f1-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="763f1-117">**Lista de dispositivos** - Selecione o nome do dispositivo na lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="763f1-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="763f1-118">**Caixa de pesquisa** - Selecione Dispositivo no menu suspenso e insira o nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="763f1-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="763f1-119">Você também pode acessar a página de alertas através do modo de exibição de arquivo e IP.</span><span class="sxs-lookup"><span data-stu-id="763f1-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="763f1-120">Selecione **Gerenciar Marcas** na linha de ações de Resposta.</span><span class="sxs-lookup"><span data-stu-id="763f1-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="763f1-121">Digitar para localizar ou criar marcas.</span><span class="sxs-lookup"><span data-stu-id="763f1-121">Type to find or create tags.</span></span>

<span data-ttu-id="763f1-122">As marcas são adicionadas ao modo de exibição do dispositivo e são refletidas no modo de exibição de lista Dispositivos.</span><span class="sxs-lookup"><span data-stu-id="763f1-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="763f1-123">Depois, você poderá usar o filtro Marcas para ver a lista relevante de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="763f1-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="763f1-124">Para saber mais, veja [Criar e gerenciar marcas de dispositivo](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="763f1-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>