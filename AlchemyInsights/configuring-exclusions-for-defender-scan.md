---
title: Configurando exclusões para verificação da Proteção Avançada contra Ameaças do Microsoft Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768320"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="b3f21-102">Configurando exclusões para verificação da Proteção Avançada contra Ameaças do Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="b3f21-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="b3f21-103">Em geral, você pode excluir certas extensões de arquivo e locais de pasta das verificações da Proteção Avançada contra Ameaças do Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="b3f21-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="b3f21-104">Você também pode configurar exclusões para arquivos abertos por certos processos.</span><span class="sxs-lookup"><span data-stu-id="b3f21-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="b3f21-105">Para mais informações, consulte [Configurar e validar exclusões com base na extensão do arquivo e local da pasta](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) e [Configurar exclusões para arquivos abertos por processos](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="b3f21-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="b3f21-106">Para configurar exclusões para o **Windows Server 2016 e 2019**, consulte [Configurar as exclusões do Microsoft Defender Antivirus no Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="b3f21-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="b3f21-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="b3f21-107">**Mac**</span></span>

<span data-ttu-id="b3f21-108">Para obter detalhes sobre os tipos de exclusão suportados e configuração de uma lista de exclusões para Mac, consulte [Tipos de exclusão suportados](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) e [Como configurar a lista de exclusões](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="b3f21-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="b3f21-109">**Observação** Você também pode validar listas de exclusões usando o arquivo de teste EICAR.</span><span class="sxs-lookup"><span data-stu-id="b3f21-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="b3f21-110">Para mais informações, consulte [Validar listas de exclusões com o arquivo de teste EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)..</span><span class="sxs-lookup"><span data-stu-id="b3f21-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="b3f21-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="b3f21-111">**Linux**</span></span>

<span data-ttu-id="b3f21-112">Para obter detalhes sobre os tipos de exclusão suportados e a configuração de uma lista de exclusões para Linux, consulte [Tipos de exclusão suportados](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) e [Configurar e validar exclusões para o Microsoft Defender ATP para Linux ](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="b3f21-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="b3f21-113">**Observação** Você também pode validar listas de exclusões usando o arquivo de teste EICAR.</span><span class="sxs-lookup"><span data-stu-id="b3f21-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="b3f21-114">Para mais informações, consulte [Validar listas de exclusões com o arquivo de teste EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="b3f21-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 