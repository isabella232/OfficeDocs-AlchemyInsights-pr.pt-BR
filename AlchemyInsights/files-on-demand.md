---
title: Arquivos Sob Demanda
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745297"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="ac052-102">Configurar Arquivos Sob Demanda</span><span class="sxs-lookup"><span data-stu-id="ac052-102">Configure Files On-Demand</span></span>

<span data-ttu-id="ac052-103">Os Arquivos do OneDrive Sob Demanda ajudam a acessar todos os arquivos no OneDrive sem precisar baixá-los nem usar o espaço de armazenamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac052-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="ac052-104">Para configurar os Arquivos Sob Demanda em seu computador:</span><span class="sxs-lookup"><span data-stu-id="ac052-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="ac052-105">Selecione o ícone de nuvem branca ou azul do **OneDrive** na área de notificação da barra de tarefas do Windows.</span><span class="sxs-lookup"><span data-stu-id="ac052-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="ac052-106">Selecione **Configurações e ajuda** ícone de engrenagem > **Configurações**.</span><span class="sxs-lookup"><span data-stu-id="ac052-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="ac052-107">Na guia **Configurações**, selecione a caixa **Economizar espaço e baixar os arquivos à medida que os usar**.</span><span class="sxs-lookup"><span data-stu-id="ac052-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="ac052-108">Você também pode configurar os Arquivos Sob Demanda usando o registro.</span><span class="sxs-lookup"><span data-stu-id="ac052-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="ac052-109">Se você desabilitar essa configuração, os usuários do Windows 10 terão o mesmo comportamento de sincronização que os usuários de versões anteriores do Windows e não poderão ativar os Arquivos Sob Demanda.</span><span class="sxs-lookup"><span data-stu-id="ac052-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="ac052-110">Se você não definir essa configuração, os usuários podem ativar ou desativar os Arquivos Sob Demanda.</span><span class="sxs-lookup"><span data-stu-id="ac052-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="ac052-111">Habilitar essa política define a seguinte chave do registro como 1.</span><span class="sxs-lookup"><span data-stu-id="ac052-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="ac052-112">Desabilitar essa política define a seguinte chave do registro como 0.</span><span class="sxs-lookup"><span data-stu-id="ac052-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="ac052-113">Se não conseguir ver a opção Arquivos Sob Demanda em "Configurações", certifique-se de que o tipo de início do serviço "Driver de Filtro de Arquivos do Windows Cloud" esteja definido como 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="ac052-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="ac052-114">A habilitação deste recurso define o seguinte valor da chave do registro como 2.</span><span class="sxs-lookup"><span data-stu-id="ac052-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`