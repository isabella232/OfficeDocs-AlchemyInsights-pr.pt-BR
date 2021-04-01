---
title: Definir o Microsoft Edge como o navegador padrão em um dispositivo ingressado em um domínio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426762"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="a4c6c-102">Definir o Microsoft Edge como o navegador padrão em um dispositivo ingressado em um domínio</span><span class="sxs-lookup"><span data-stu-id="a4c6c-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="a4c6c-103">Definir Microsoft Edge como o navegador padrão:</span><span class="sxs-lookup"><span data-stu-id="a4c6c-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="a4c6c-104">[Criar um arquivo de configuração de associações padrão](https://go.microsoft.com/fwlink/?linkid=2132437) e armazená-lo localmente ou em um compartilhamento de rede.</span><span class="sxs-lookup"><span data-stu-id="a4c6c-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="a4c6c-105">Abra o editor de Políticas de Grupo, e depois vá para **Configuração do Computador** > **Modelos Administrativos** > **Componentes do Windows** > **Explorador de Arquivos**.</span><span class="sxs-lookup"><span data-stu-id="a4c6c-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="a4c6c-106">Selecione **Configurar um arquivo padrão de configuração de associações**.</span><span class="sxs-lookup"><span data-stu-id="a4c6c-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="a4c6c-107">Selecione **Configuração de política**, e depois selecione **Habilitado**.</span><span class="sxs-lookup"><span data-stu-id="a4c6c-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="a4c6c-108">Em **Opções**, digite a localização do seu arquivo de configuração de associações padrão e selecione **OK**.</span><span class="sxs-lookup"><span data-stu-id="a4c6c-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
