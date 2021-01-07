---
title: Proteção de dataprotection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768805"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="128da-102">Habilitando a criptografia BitLocker com o Intune</span><span class="sxs-lookup"><span data-stu-id="128da-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="128da-103">A política do Intune Endpoint Protection pode ser usada para definir as configurações de criptografia do BitLocker para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="128da-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="128da-104">Para obter mais informações, consulte [configurações do Windows 10 (e posteriores) para proteger dispositivos usando o Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="128da-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="128da-105">Você deve estar ciente de que muitos dispositivos mais recentes executando o Windows 10 dão suporte à criptografia automática do BitLocker, que é disparada sem a aplicação da política MDM.</span><span class="sxs-lookup"><span data-stu-id="128da-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="128da-106">Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas.</span><span class="sxs-lookup"><span data-stu-id="128da-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="128da-107">Consulte as perguntas frequentes a seguir para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="128da-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="128da-108">Para obter informações sobre a solução de problemas do BitLocker, consulte [Troubleshoot BitLocker Policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="128da-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="128da-109">**Perguntas Frequentes**</span><span class="sxs-lookup"><span data-stu-id="128da-109">**FAQ**</span></span>

<span data-ttu-id="128da-110">P: Quais edições do Windows dão suporte à criptografia de dispositivo usando a política do Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="128da-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="128da-111">A: as configurações na política do Intune Endpoint Protection são implementadas usando o [CSP do BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="128da-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="128da-112">Nem todas as edições ou versões do Windows dão suporte ao CSP do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="128da-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="128da-113">P: como o BitLocker pode ser habilitado nos dispositivos sem exigir interação do usuário final?</span><span class="sxs-lookup"><span data-stu-id="128da-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="128da-114">A: desde que os pré-requisitos necessários sejam atendidos, é possível habilitar a "criptografia silenciosa" do BitLocker por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="128da-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="128da-115">Consulte os detalhes dos requisitos do dispositivo e as configurações de política de exemplo para habilitar a criptografia silenciosa no seguinte documento: [habilitar a criptografia BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)de forma silenciosa.</span><span class="sxs-lookup"><span data-stu-id="128da-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="128da-116">P: se um dispositivo já estiver criptografado com o BitLocker usando as configurações padrão do sistema operacional para o método de criptografia e o nível de codificação (XTS-AES-128), a aplicação de uma política com configurações diferentes disparará novamente a criptografia da unidade com as novas configurações?</span><span class="sxs-lookup"><span data-stu-id="128da-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="128da-117">R: Não.</span><span class="sxs-lookup"><span data-stu-id="128da-117">A: No.</span></span> <span data-ttu-id="128da-118">Para aplicar as novas configurações de codificação, a unidade deve primeiro ser descriptografada.</span><span class="sxs-lookup"><span data-stu-id="128da-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="128da-119">**Observação:** Para os dispositivos que estão sendo registrados com o AutoPilot, a criptografia automática que ocorre durante o OOBE não é disparada até que a política do Intune seja avaliada, o que permite que as configurações baseadas em políticas sejam usadas no lugar dos padrões do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="128da-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="128da-120">P: se um dispositivo for criptografado como resultado do aplicativo da política do Intune, ele será descriptografado quando essa política for removida?</span><span class="sxs-lookup"><span data-stu-id="128da-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="128da-121">A: a remoção da política relacionada à criptografia não resulta na descriptografia das unidades que foram configuradas.</span><span class="sxs-lookup"><span data-stu-id="128da-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="128da-122">P: por que a política de conformidade do Intune mostra que meu dispositivo não tem o BitLocker habilitado, embora seja?</span><span class="sxs-lookup"><span data-stu-id="128da-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="128da-123">A: a configuração "BitLocker Enabled" na política de conformidade do Intune utiliza o cliente do atestado de integridade do dispositivo Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="128da-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="128da-124">Este cliente só mede o estado do dispositivo no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="128da-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="128da-125">Portanto, se um dispositivo não tiver sido reiniciado desde que a criptografia BitLocker foi concluída, o serviço de cliente DHA não relatará o BitLocker como ativo.</span><span class="sxs-lookup"><span data-stu-id="128da-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 