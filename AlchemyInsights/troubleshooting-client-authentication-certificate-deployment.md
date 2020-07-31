---
title: Solução de problemas na implantação do certificado de autenticação do cliente
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509036"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="bf2d9-102">Solução de problemas na implantação do certificado de autenticação do cliente</span><span class="sxs-lookup"><span data-stu-id="bf2d9-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="bf2d9-103">Os perfis Intune NDES/SCEP e PKCS/PFX de certificados de clientes são normalmente usados em conjunto com outros tipos de perfis, como Wi-Fi, VPN e e-mails, para permitir que os usuários autentiquem os recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="bf2d9-104">Quando esses tipos de perfil estão ligados a um perfil de certificado de cliente, dependem do sucesso da implantação desse perfil.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="bf2d9-105">A configuração inicial da infraestrutura e a configuração associada do perfil do Certificado do cliente normalmente exigem a solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="bf2d9-106">Para obter um guia passo a passo para a configuração bem-sucedida do conector NDES e orientações de solução de problemas para isolar problemas com a implantação de certificados, consulte:</span><span class="sxs-lookup"><span data-stu-id="bf2d9-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="bf2d9-107">Configurar a infraestrutura para oferecer suporte ao SCEP com o Intune</span><span class="sxs-lookup"><span data-stu-id="bf2d9-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="bf2d9-108">Visão geral da solução de problemas dos perfis de certificados SCEP com o Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bf2d9-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="bf2d9-109">Usar os scripts do Powershell referenciados para ajudar a verificar sua configuração.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="bf2d9-110">Para obter ais informações, consulte [Scripts de verificação de conectores Intune Certificate](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="bf2d9-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="bf2d9-111">**Outros problemas comuns**</span><span class="sxs-lookup"><span data-stu-id="bf2d9-111">**Other common issues**</span></span>

<span data-ttu-id="bf2d9-112">**Quando tento instalar o conector do certificado Intune no servidor do conector NDES, recebo a mensagem: "A senha no pedido de certificado não pode ser verificada. Ela já pode ter sido usada. Obtenha uma nova senha para enviar com esta solicitação".**</span><span class="sxs-lookup"><span data-stu-id="bf2d9-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="bf2d9-113">Essa mensagem quer dizer que você precisa executar a instalação do conector do certificado como Administrador.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="bf2d9-114">Em alguns ambientes, os servidores onde o Certificado Intune é executado devem usar um servidor proxy para se conectarem ao Intune e, assim, o Conector do Certificado deve usar um proxy.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="bf2d9-115">Em algumas circunstâncias, o Conector NDES ignora as configurações de proxy configuradas, e talvez seja necessário configurar as configurações de proxy enquanto estiver em execução no contexto de segurança do LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="bf2d9-116">A solução é executar o Internet Explorer como SISTEMA e configurar um proxy no IE.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="bf2d9-117">Depois de reiniciar o Serviço de Conector Intune, o Conector NDES se conecta ao Intune.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="bf2d9-118">**Os dispositivos do usuário não estão mais recebendo certificados SCEP da NDES.**</span><span class="sxs-lookup"><span data-stu-id="bf2d9-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="bf2d9-119">É possível que o certificado de Autenticação do Cliente emitido para o servidor NDES, e especificado durante a instalação do conector NDES, tenha expirado ou esteja desaparecido.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="bf2d9-120">Para resolver:</span><span class="sxs-lookup"><span data-stu-id="bf2d9-120">To resolve:</span></span> 
 
1. <span data-ttu-id="bf2d9-121">Desinstalar o conector NDES.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="bf2d9-122">Usar estes detalhes para solicitar uma nova autenticação de cliente ou um certificado de autenticação de servidor:</span><span class="sxs-lookup"><span data-stu-id="bf2d9-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="bf2d9-123">Nome do assunto: CN=fqdn externo</span><span class="sxs-lookup"><span data-stu-id="bf2d9-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="bf2d9-124">Nome alternativo ao assunto (ambos são necessários): DNS=fqdn externo, DNS=fqdn interno</span><span class="sxs-lookup"><span data-stu-id="bf2d9-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="bf2d9-125">Reinstalar o conector NDES com o novo certificado.</span><span class="sxs-lookup"><span data-stu-id="bf2d9-125">Reinstall the NDES connector with the new certificate.</span></span>