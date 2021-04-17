---
title: Mitigar o erro O aplicativo não foi detectado
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
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836339"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="05c58-102">Mitigar o erro "O aplicativo não foi detectado"</span><span class="sxs-lookup"><span data-stu-id="05c58-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="05c58-103">O erro de instalação de aplicativo "O aplicativo não foi detectado após a instalação bem-sucedida", relatado pelo Intune, pode ocorrer em todas as principais plataformas de sistema operacional (Windows, iOS e Android).</span><span class="sxs-lookup"><span data-stu-id="05c58-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="05c58-104">Os cenários mais comuns que geram esse erro incluem:</span><span class="sxs-lookup"><span data-stu-id="05c58-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="05c58-105">O aplicativo foi atualizado fora do Intune (a partir de uma loja de aplicativos de terceiros) após a implantação inicial.</span><span class="sxs-lookup"><span data-stu-id="05c58-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="05c58-106">Por exemplo, alguns aplicativos, como o Google Chrome, podem executar atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="05c58-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="05c58-107">Um usuário desinstalou o aplicativo após a instalação inicial.</span><span class="sxs-lookup"><span data-stu-id="05c58-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="05c58-108">Para corrigir esse problema, primeiro execute uma análise dos dispositivos afetados para determinar o cenário em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="05c58-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="05c58-109">Se o aplicativo tiver sido atualizado fora do Intune, a implantação de aplicativos poderá ser configurada para ignorar a versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="05c58-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="05c58-110">Para fazer isso, em **Configuração do Aplicativo > Informações do Aplicativo,**, defina **Ignorar versão do aplicativo** como **Sim**.</span><span class="sxs-lookup"><span data-stu-id="05c58-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="05c58-111">Ao direcionar o cliente, pode ser apropriado implantar o aplicativo como "necessário", além de garantir que a versão mais recente tenha sido implantada.</span><span class="sxs-lookup"><span data-stu-id="05c58-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="05c58-112">Como alternativa, na plataforma iOS, é possível usar a funcionalidade **AutoUpdate** associada ao Programa de Compra de Volume Apple, que pode ser configurada para atualizar automaticamente para novas versões do aplicativo à medida que elas são disponibilizadas.</span><span class="sxs-lookup"><span data-stu-id="05c58-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="05c58-113">Para obter mais informações sobre como solucionar problemas de instalação do aplicativo, confira [Solucionar problemas de instalação do aplicativo](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="05c58-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
