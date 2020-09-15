---
title: Inventário de dispositivos do Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667866"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="eb40b-102">Inventário de dispositivos do Intune</span><span class="sxs-lookup"><span data-stu-id="eb40b-102">Intune Device Inventory</span></span>

<span data-ttu-id="eb40b-103">A lâmina de Dispositivos fornece ao administrador uma visão geral dos dispositivos em gerenciamento do Intune por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb40b-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="eb40b-104">As informações mostradas incluem: hardware, aplicativos descobertos, estado de conformidade de dispositivos e estado de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb40b-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="eb40b-105">Os dados de inventário para hardware e aplicativos descobertos são coletados em um ciclo de sete dias.</span><span class="sxs-lookup"><span data-stu-id="eb40b-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="eb40b-106">Os aplicativos e os elementos específicos do hardware relatado são diferentes dependendo do sistema operacional do dispositivo e se o dispositivo é pessoal ou corporativo.</span><span class="sxs-lookup"><span data-stu-id="eb40b-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="eb40b-107">Para obter mais informações, confira [Ver detalhes do dispositivo no Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="eb40b-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="eb40b-108">**Perguntas Frequentes**</span><span class="sxs-lookup"><span data-stu-id="eb40b-108">**FAQ**</span></span>

<span data-ttu-id="eb40b-109">P: Não estou recebendo uma lista completa de inventários dos aplicativos presentes nos dispositivos Windows registrados no Intune.</span><span class="sxs-lookup"><span data-stu-id="eb40b-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="eb40b-110">Por que não?</span><span class="sxs-lookup"><span data-stu-id="eb40b-110">Why not?</span></span>

<span data-ttu-id="eb40b-111">R: No momento, somente os aplicativos modernos estão listados para PCs com Windows 10, identificados como dispositivos corporativos.</span><span class="sxs-lookup"><span data-stu-id="eb40b-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="eb40b-112">O Intune não coletará informações sobre aplicativos Win32 instalados nesses dispositivos.</span><span class="sxs-lookup"><span data-stu-id="eb40b-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="eb40b-113">P: Por que os números de telefone não são coletados em todos os dispositivos?</span><span class="sxs-lookup"><span data-stu-id="eb40b-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="eb40b-114">R: Os telefones classificados como dispositivos corporativos no Intune não serão identificados com o número de telefone inteiro quando, por exemplo, você executar um relatório de inventário de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="eb40b-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="eb40b-115">Os números de telefone de todos os dispositivos são sempre mascarados parcialmente por asteriscos (\*\*\*\*) e mostram somente os últimos quatro dígitos.</span><span class="sxs-lookup"><span data-stu-id="eb40b-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>