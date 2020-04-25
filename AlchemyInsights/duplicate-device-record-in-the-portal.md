---
title: Registro de dispositivo duplicado no portal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789551"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="1f899-102">Registro de dispositivo duplicado no portal</span><span class="sxs-lookup"><span data-stu-id="1f899-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="1f899-103">Você pode ver dois registros de um dispositivo no portal se o dispositivo não relatar corretamente o status de cogerenciamento no site do Gerenciador de Configurações.</span><span class="sxs-lookup"><span data-stu-id="1f899-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="1f899-104">Para verificar o status de cogerenciamento de um dispositivo, verifique a coluna **Cogerenciado** para o dispositivo no console do Gerenciador de Configurações.</span><span class="sxs-lookup"><span data-stu-id="1f899-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="1f899-105">Se a coluna não estiver visível, você poderá adicioná-la clicando com o botão direito do mouse em qualquer um dos cabeçalhos da coluna e selecionando-a na lista.</span><span class="sxs-lookup"><span data-stu-id="1f899-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="1f899-106">O valor cogerenciado deve ser **Sim**.</span><span class="sxs-lookup"><span data-stu-id="1f899-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="1f899-107">Se o valor for **Não**, abra o miniaplicativo de cliente do Gerenciador de Configurações no dispositivo do cliente e verifique a propriedade **Cogerenciamento** na guia Geral.</span><span class="sxs-lookup"><span data-stu-id="1f899-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="1f899-108">Se o valor estiver **Habilitado**, isso indicará problemas com a comunicação do cliente com o Ponto de Gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1f899-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="1f899-109">Verifique o **CcmMessaging.log** no dispositivo para investigar possíveis problemas de conectividade.</span><span class="sxs-lookup"><span data-stu-id="1f899-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="1f899-110">Se o valor estiver **Desabilitado** e o dispositivo estiver registrado no Intune, certifique-se de que o dispositivo recebeu a política de gerenciamento de cogerenciamento verificando o\*\* CoManagementHandler.log\*\* no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1f899-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
