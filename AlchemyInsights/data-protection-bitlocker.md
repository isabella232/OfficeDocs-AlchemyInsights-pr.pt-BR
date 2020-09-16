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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731227"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="21249-102">Habilitando a criptografia BitLocker com o Intune</span><span class="sxs-lookup"><span data-stu-id="21249-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="21249-103">A política do Intune Endpoint Protection pode ser usada para definir as configurações de criptografia do BitLocker para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="21249-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="21249-104">Para obter mais informações, consulte [configurações do Windows 10 (e posteriores) para proteger dispositivos usando o Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="21249-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="21249-105">Você deve estar ciente de que muitos dispositivos mais recentes executando o Windows 10 dão suporte à criptografia automática do BitLocker, que é disparada sem a aplicação da política MDM.</span><span class="sxs-lookup"><span data-stu-id="21249-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="21249-106">Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas.</span><span class="sxs-lookup"><span data-stu-id="21249-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="21249-107">Consulte as perguntas frequentes a seguir para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="21249-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="21249-108">Para obter informações sobre a solução de problemas do BitLocker, consulte [Troubleshoot BitLocker Policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="21249-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="21249-109">**Perguntas Frequentes**</span><span class="sxs-lookup"><span data-stu-id="21249-109">**FAQ**</span></span>

 <span data-ttu-id="21249-110">P: Quais edições do Windows dão suporte à criptografia de dispositivo usando a política do Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="21249-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="21249-111">A: as configurações na política do Intune Endpoint Protection são implementadas usando o [CSP do BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="21249-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="21249-112">Nem todas as edições ou versões do Windows dão suporte ao CSP do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="21249-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="21249-113">No momento, as seguintes edições do Windows têm suporte: Enterprise, Education, Mobile, Mobile Enterprise e Professional (Build 1809 e posterior).</span><span class="sxs-lookup"><span data-stu-id="21249-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="21249-114">P: se um dispositivo já estiver criptografado com o BitLocker usando as configurações padrão do sistema operacional para o método de criptografia e o nível de codificação (XTS-AES-128), a aplicação de uma política com configurações diferentes disparará novamente a criptografia da unidade com as novas configurações?</span><span class="sxs-lookup"><span data-stu-id="21249-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="21249-115">R: Não.</span><span class="sxs-lookup"><span data-stu-id="21249-115">A: No.</span></span> <span data-ttu-id="21249-116">Para aplicar as novas configurações de codificação, a unidade deve primeiro ser descriptografada.</span><span class="sxs-lookup"><span data-stu-id="21249-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="21249-117">**Observação:** Para os dispositivos que estão sendo registrados com o AutoPilot, a criptografia automática que ocorre durante o OOBE não é disparada até que a política do Intune seja avaliada, o que permite que as configurações baseadas em políticas sejam usadas no lugar dos padrões do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="21249-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="21249-118">P: se um dispositivo for criptografado como resultado do aplicativo da política do Intune, ele será descriptografado quando essa política for removida?</span><span class="sxs-lookup"><span data-stu-id="21249-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="21249-119">A: a remoção da política relacionada à criptografia não resulta na descriptografia das unidades que foram configuradas.</span><span class="sxs-lookup"><span data-stu-id="21249-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="21249-120">P: por que a política de conformidade do Intune mostra que meu dispositivo não tem o BitLocker habilitado, embora seja?</span><span class="sxs-lookup"><span data-stu-id="21249-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="21249-121">A: a configuração "BitLocker Enabled" na política de conformidade do Intune utiliza o cliente do atestado de integridade do dispositivo Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="21249-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="21249-122">Este cliente só mede o estado do dispositivo no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="21249-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="21249-123">Portanto, se um dispositivo não tiver sido reiniciado desde que a criptografia BitLocker foi concluída, o serviço de cliente DHA não relatará o BitLocker como ativo.</span><span class="sxs-lookup"><span data-stu-id="21249-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 