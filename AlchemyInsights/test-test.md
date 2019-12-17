---
title: Termos ausentes do repositório de termos do SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053501"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="5fded-102">Habilitando a criptografia BitLocker com o Intune</span><span class="sxs-lookup"><span data-stu-id="5fded-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="5fded-103">A política do Intune Endpoint Protection pode ser usada para definir configurações de criptografia do Boitlocker para dispositivos Windows, conforme descrito em: Windows10 (e posterior) configurações para proteger dispositivos usando o Intune</span><span class="sxs-lookup"><span data-stu-id="5fded-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="5fded-104">Você deve estar ciente de que muitos dispositivos mais recentes que executam o Windows 10 dão suporte à criptografia automática do BitLocker, que é disparada sem a aplicação da política de MDM.</span><span class="sxs-lookup"><span data-stu-id="5fded-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="5fded-105">Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas.</span><span class="sxs-lookup"><span data-stu-id="5fded-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="5fded-106">Confira mais detalhes na seção perguntas frequentes.</span><span class="sxs-lookup"><span data-stu-id="5fded-106">See FAQ for more detail.</span></span>


<span data-ttu-id="5fded-107">Perguntas  frequentes p: Quais edições do Windows dão suporte à criptografia de dispositivo usando a política do Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="5fded-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="5fded-108"> A: as configurações na política do Intune Endpoint Protection são implementadas usando o CSP do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="5fded-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="5fded-109">Nem todas as edições nem versões do Windows dão suporte ao CSP do BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="5fded-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="5fded-110">No momento, edições do Windows: Enterprise; Educação, Mobile, Mobile Enterprise e Professional (da compilação 1809 em diante) são suportados.</span><span class="sxs-lookup"><span data-stu-id="5fded-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="5fded-111">P: se um dispositivo já estiver criptografado com o BitLocker usando as configurações padrão do sistema operacional para o método de criptografia e o nível de codificação (XTS-AES-128), a aplicação de uma política com configurações diferentes disparará novamente a criptografia da unidade com as novas configurações?</span><span class="sxs-lookup"><span data-stu-id="5fded-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="5fded-112">R: Não.</span><span class="sxs-lookup"><span data-stu-id="5fded-112">A: No.</span></span> <span data-ttu-id="5fded-113">Para aplicar as novas configurações de codificação, a unidade deve primeiro ser descriptografada.</span><span class="sxs-lookup"><span data-stu-id="5fded-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="5fded-114">Observação para os dispositivos que estão sendo registrados com o AutoPilot a criptografia automática que ocorre durante o OOBE não é disparada até que a política do Intune seja avaliada, o que permite que as configurações baseadas em políticas sejam usadas no lugar dos padrões do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="5fded-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="5fded-115">P se um dispositivo for criptografado como resultado do aplicativo da política do Intune, ele será descriptografado quando essa política for removida?</span><span class="sxs-lookup"><span data-stu-id="5fded-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="5fded-116">A: a remoção da política relacionada à criptografia não resulta na descriptografia das unidades que foram configuradas.</span><span class="sxs-lookup"><span data-stu-id="5fded-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="5fded-117">P: por que a política de conformidade do Intune mostra que meu dispositivo não tem "BitLocker habilitado", mas é?</span><span class="sxs-lookup"><span data-stu-id="5fded-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="5fded-118">A: a configuração "BitLocker Enabled" na política de conformidade do Intune utiliza o cliente do atestado de integridade do dispositivo Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="5fded-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="5fded-119">Este cliente só mede o estado do dispositivo no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="5fded-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="5fded-120">Portanto, se um dispositivo não tiver sido reiniciado desde que a criptografia BitLocker foi concluída, o serviço de cliente DHA não relatará o BitLocker como ativo.</span><span class="sxs-lookup"><span data-stu-id="5fded-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>