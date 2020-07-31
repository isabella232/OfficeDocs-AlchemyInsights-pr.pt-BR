---
title: Perfis Wi-Fi do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509037"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="e4787-102">Perfis Wi-Fi do Intune</span><span class="sxs-lookup"><span data-stu-id="e4787-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="e4787-103">A implementação bem sucedida da conectividade Wi-Fi para clientes MDM depende de um perfil corretamente implantado que reflita as exigências da infraestrutura de Wi-Fi corporativa.</span><span class="sxs-lookup"><span data-stu-id="e4787-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="e4787-104">Para rever as configurações apropriadas das plataformas do cliente que você está investigando, consulte:</span><span class="sxs-lookup"><span data-stu-id="e4787-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="e4787-105">Adicionar configurações Wi-Fi aos dispositivos com Android no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e4787-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="e4787-106">Adicionar configurações Wi-Fi aos dispositivos dedicados e totalmente gerenciados do Android Enterprise no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e4787-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="e4787-107">Adicionar configurações Wi-Fi aos dispositivos iOS e iPadOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e4787-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="e4787-108">Adicionar configurações Wi-Fi ao Windows 10 e dispositivos posteriores no Intune</span><span class="sxs-lookup"><span data-stu-id="e4787-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="e4787-109">Importar configurações Wi-Fi aos dispositivos Windows no Intune</span><span class="sxs-lookup"><span data-stu-id="e4787-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="e4787-110">**Problemas comuns**</span><span class="sxs-lookup"><span data-stu-id="e4787-110">**Common Issues**</span></span>

<span data-ttu-id="e4787-111">**Estou implantando um perfil de Wi-Fi que depende de um certificado de implantação especificado no perfil de Wi-Fi. Entretanto, os perfis de configuração estão exibindo um status de erro.**</span><span class="sxs-lookup"><span data-stu-id="e4787-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="e4787-112">Verifique se o seu dispositivo recebeu o certificado.</span><span class="sxs-lookup"><span data-stu-id="e4787-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="e4787-113">No Intune, acesse **Todos os dispositivos** e selecione o dispositivo > **Configuração do dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="e4787-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="e4787-114">Verifique se todos os perfis esperados estão listados e em um estado bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="e4787-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="e4787-115">Quanto a um perfil do Android, se você tiver certificados intermediários na sua cadeia de certificados, certifique-se de que eles sejam implantados nos dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="e4787-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="e4787-116">Para verificar o status do certificado, acesse **Configuração do dispositivo** > **Perfis** > **AC intermediário do Android** > **Propriedades** > **Certificado de confiança**.</span><span class="sxs-lookup"><span data-stu-id="e4787-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="e4787-117">Se você continuar a visualizar erros, reveja os procedimentos e as seções de solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="e4787-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="e4787-118">Para obter mais informações, consulte [Visão geral da solução de problemas dos perfis de certificados SCEP com o Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e4787-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="e4787-119">**Eu implantei um perfil de Wi-Fi em um dispositivo. O Intune está mostrando que foi bem sucedido, mas o dispositivo não está se conectando ao Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="e4787-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="e4787-120">Um status de sucesso significa que o Intune implantou com sucesso o perfil conforme configurado.</span><span class="sxs-lookup"><span data-stu-id="e4787-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="e4787-121">Entretanto, talvez essas configurações não correspondam aos requisitos de sua rede e/ou autenticação.</span><span class="sxs-lookup"><span data-stu-id="e4787-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="e4787-122">Para obter mais detalhes sobre a tentativa de conexão, revise os logs na infraestrutura e no serviço de autenticação (no controlador do ponto de acesso de Wi-Fi e no servidor NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="e4787-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="e4787-123">Talvez você tenha que trabalhar com sua equipe de infraestrutura de rede ou com o fornecedor de Wi-Fi de terceiros para reunir e revisar os logs.</span><span class="sxs-lookup"><span data-stu-id="e4787-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>