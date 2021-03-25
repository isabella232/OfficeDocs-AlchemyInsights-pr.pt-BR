---
title: Ajuda com a configuração de luz noturna
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123012"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="a048e-102">Ajuda com a configuração de luz noturna</span><span class="sxs-lookup"><span data-stu-id="a048e-102">Help with the night light display setting</span></span>

<span data-ttu-id="a048e-103">Para saber mais sobre as configurações de exibição noturna, consulte [Agendar a exibição noturna no Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="a048e-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="a048e-104">Se as opções de luz noturna estiverem desativadas em Configurações, verifique o driver de vídeo:</span><span class="sxs-lookup"><span data-stu-id="a048e-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="a048e-105">Clique na caixa de pesquisa na barra de tarefas e digite **Gerenciador de Dispositivos** e selecione **Gerenciador de Dispositivos** nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a048e-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="a048e-106">Expanda **adaptadores de vídeo**.</span><span class="sxs-lookup"><span data-stu-id="a048e-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="a048e-107">Infelizmente, o recurso de luz noturna não estará disponível se o seu dispositivo usar um driver DisplayLink ou Basic Display.</span><span class="sxs-lookup"><span data-stu-id="a048e-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="a048e-108">O recurso de luz noturna usa tecnologia gráfica recente, portanto, pode ser necessário atualizar o driver de vídeo:</span><span class="sxs-lookup"><span data-stu-id="a048e-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="a048e-109">Verifique se há atualizações em **Iniciar** > **Configurações** > **Atualização e Segurança** > **Windows Update** > **Verificar se há atualizações**.</span><span class="sxs-lookup"><span data-stu-id="a048e-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="a048e-110">OU</span><span class="sxs-lookup"><span data-stu-id="a048e-110">OR</span></span>

- <span data-ttu-id="a048e-111">Visite o site de suporte do fabricante de hardware para baixar e instalar manualmente os drivers de vídeo mais recentes.</span><span class="sxs-lookup"><span data-stu-id="a048e-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="a048e-112">Redefinir o modo de luz noturna no registro</span><span class="sxs-lookup"><span data-stu-id="a048e-112">Reset night light in the registry</span></span>

<span data-ttu-id="a048e-113">Se a atualização do driver de vídeo não funcionar, pode ser necessário redefinir o modo de luz noturna no registro.</span><span class="sxs-lookup"><span data-stu-id="a048e-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="a048e-114">**Cuidado:** esta etapa da solução de problemas é recomendada apenas para usuários avançados.</span><span class="sxs-lookup"><span data-stu-id="a048e-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="a048e-115">Problemas graves podem ocorrer se você modificar o registro incorretamente.</span><span class="sxs-lookup"><span data-stu-id="a048e-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="a048e-116">Para ter mais proteção, faça backup do registro antes de modificá-lo para que possa restaurá-lo se ocorrerem problemas.</span><span class="sxs-lookup"><span data-stu-id="a048e-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="a048e-117">Na caixa de pesquisa, digite **regedit** e selecione **Editor do Registro** nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a048e-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="a048e-118">Vá para a seguinte chave de registro:</span><span class="sxs-lookup"><span data-stu-id="a048e-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="a048e-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="a048e-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="a048e-120">Exporte e exclua a seguinte subchave:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="a048e-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="a048e-121">Exporte e exclua a seguinte subchave:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="a048e-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="a048e-122">Reinicie o Windows e verifique se as opções de luz noturna estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a048e-122">Restart Windows and verify if the night light options are available.</span></span>


