---
title: Problemas relacionados à VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505173"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="2d662-102">Problemas relacionados à VPN</span><span class="sxs-lookup"><span data-stu-id="2d662-102">VPN related issues</span></span>

<span data-ttu-id="2d662-103">A implementação bem-sucedida da conectividade VPN para clientes MDM depende de um perfil implantado que reflete corretamente os requisitos da infraestrutura VPN.</span><span class="sxs-lookup"><span data-stu-id="2d662-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="2d662-104">Para configurar adequadamente as plataformas de cliente que está investigando, confira:</span><span class="sxs-lookup"><span data-stu-id="2d662-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="2d662-105">Configurações de dispositivo do Windows 10 e Windows Holographic para adicionar conexões de VPN usando o Intune</span><span class="sxs-lookup"><span data-stu-id="2d662-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="2d662-106">Adicionar configurações de VPN a dispositivos iOS e iPadOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2d662-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="2d662-107">Configurações de dispositivo Android para configurar a VPN no Intune</span><span class="sxs-lookup"><span data-stu-id="2d662-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="2d662-108">Adicionar configurações de VPN a dispositivos macOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2d662-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="2d662-109">Se seu perfil VPN usar autenticação baseada em certificado, garanta que o certificado raiz e os perfis de certificado de autenticação de cliente vinculados ao perfil VPN sejam implantados com êxito.</span><span class="sxs-lookup"><span data-stu-id="2d662-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="2d662-110">**Problemas Comuns**</span><span class="sxs-lookup"><span data-stu-id="2d662-110">**Common Issues**</span></span>

<span data-ttu-id="2d662-111">**Implantei um perfil VPN em um dispositivo. O Intune está mostrando que foi bem-sucedido, mas o dispositivo não está se conectando à VPN.**</span><span class="sxs-lookup"><span data-stu-id="2d662-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="2d662-112">Um status bem-sucedido significa que o Intune implantou o perfil configurado com êxito.</span><span class="sxs-lookup"><span data-stu-id="2d662-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="2d662-113">No entanto, essas configurações podem não corresponder aos requisitos de rede e/ou autenticação.</span><span class="sxs-lookup"><span data-stu-id="2d662-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="2d662-114">Examine os logs no serviço de infraestrutura e de autenticação (no servidor VPN e no servidor NPS/Radius) para obter mais detalhes sobre a tentativa de conexão.</span><span class="sxs-lookup"><span data-stu-id="2d662-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="2d662-115">Talvez você precise trabalhar com sua equipe de infraestrutura de rede ou com o fornecedor de VPN de terceiros para reunir e analisar os logs.</span><span class="sxs-lookup"><span data-stu-id="2d662-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="2d662-116">**Quando configuro uma VPN personalizada para iOS, o recurso VPN por aplicativo não é disponibilizado.**</span><span class="sxs-lookup"><span data-stu-id="2d662-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="2d662-117">A VPN por aplicativo para dispositivos iOS no Intune estão disponíveis no momento para uma lista específica de provedores e parceiros, que também devem atender aos pré-requisitos de certificado antes de configurar uma VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d662-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="2d662-118">Para saber mais, veja [Configurar VPN (Rede Virtual Privada) por aplicativo para dispositivos iOS/iPadOS no Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="2d662-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="2d662-119">Para saber mais informações sobre todos os tipos de conexão VPN no Intune, veja [Criar perfis VPN para se conectar aos servidores VPN no Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="2d662-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="2d662-120">**A VPN sob demanda do iOS não inicia quando um domínio configurado é acessado**</span><span class="sxs-lookup"><span data-stu-id="2d662-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="2d662-121">Para testar as configurações VPN automáticas, defina os valores a seguir:</span><span class="sxs-lookup"><span data-stu-id="2d662-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="2d662-122">Quero fazer o seguinte: **Avaliar todas as tentativas de conexão**</span><span class="sxs-lookup"><span data-stu-id="2d662-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="2d662-123">Escolha se deseja se conectar: **Conectar, se necessário**</span><span class="sxs-lookup"><span data-stu-id="2d662-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="2d662-124">Quando usuários acessam esses domínios: **destino** *nome de domínio*</span><span class="sxs-lookup"><span data-stu-id="2d662-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="2d662-125">Se a configuração acima não tiver êxito, adicione o seguinte elemento:</span><span class="sxs-lookup"><span data-stu-id="2d662-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="2d662-126">Quando essa URL estiver inatingível, force a conexão com a VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="2d662-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>