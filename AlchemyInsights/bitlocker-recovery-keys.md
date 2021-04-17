---
title: Chaves de recuperação do Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820274"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="568d4-102">Acessando chaves de recuperação do Bitlocker</span><span class="sxs-lookup"><span data-stu-id="568d4-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="568d4-103">Ao configurar configurações do Bitlocker Política de Proteção de Ponto de Extremidade do Intune, é possível definir se as informações de recuperação do Bitlocker devem ser armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="568d4-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="568d4-104">Se essa configuração estiver configurada, os dados de recuperação armazenados devem estar visíveis para um administrador do Intune como parte dos dados de registro do dispositivo na folha Dispositivos do Intune de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="568d4-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="568d4-105">Dispositivos - dispositivos do Azure AD -> "Device" OR Devices -> All Devices -> "Device" -> Recovery keys</span><span class="sxs-lookup"><span data-stu-id="568d4-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="568d4-106">Como alternativa, se houver acesso administrativo ao dispositivo em si, a chave de recuperação (Senha) poderá ser vista executando o seguinte comando de um prompt de comando elevado:</span><span class="sxs-lookup"><span data-stu-id="568d4-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="568d4-107">Se o dispositivo foi criptografado antes da inscrição no Intune, a chave de recuperação pode ter sido associada à "Conta da Microsoft" (MSA) usada para entrar no dispositivo durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="568d4-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="568d4-108">Se esse for o caso, acessar e entrar com esse MSA deve mostrar os dispositivos para os quais as chaves  https://onedrive.live.com/recoverykey de recuperação foram armazenadas.</span><span class="sxs-lookup"><span data-stu-id="568d4-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="568d4-109">Se o dispositivo foi criptografado como resultado da configuração por meio de política de grupo baseada em domínio, as informações de recuperação poderão ser armazenadas no Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="568d4-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="568d4-110">Se você configurou a política de proteção de ponto de extremidade para armazenar a chave de recuperação no Azure Active Directory, mas a chave de um dispositivo específico não foi carregada, você pode disparar o carregamento girando a chave de recuperação para esse dispositivo a partir do console do MEM.</span><span class="sxs-lookup"><span data-stu-id="568d4-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="568d4-111">Para obter detalhes, consulte [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="568d4-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

