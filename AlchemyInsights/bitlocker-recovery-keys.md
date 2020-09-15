---
title: Chaves de recuperação do BitLocker
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685874"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="35bd3-102">Acessar chaves de recuperação do BitLocker</span><span class="sxs-lookup"><span data-stu-id="35bd3-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="35bd3-103">Ao configurar a política de Endpoint Protection do Intune de configurações do BitLocker, é possível definir se as informações de recuperação do BitLocker devem ser armazenadas no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="35bd3-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="35bd3-104">Se essa configuração for configurada, os dados de recuperação armazenados deverão ser visíveis para um administrador do Intune como parte dos dados de registro do dispositivo na lâmina de dispositivos do Intune de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="35bd3-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="35bd3-105">Dispositivos-dispositivos do Azure AD-> "dispositivo" ou dispositivos-> todos os dispositivos-> "dispositivo"-> chaves de recuperação</span><span class="sxs-lookup"><span data-stu-id="35bd3-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="35bd3-106">Como alternativa, se houver acesso administrativo ao próprio dispositivo, a chave de recuperação (senha) poderá ser vista executando o seguinte comando a partir de um prompt de comando elevado:</span><span class="sxs-lookup"><span data-stu-id="35bd3-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="35bd3-107">Se o dispositivo foi criptografado antes do Enrolment no Intune, a chave de recuperação pode ter sido associada à "conta da Microsoft" (MSA) usada para entrar no dispositivo durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="35bd3-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="35bd3-108">Se esse for o caso, acessar  https://onedrive.live.com/recoverykey e entrar com esse MSA deve mostrar os dispositivos para os quais as chaves de recuperação foram armazenadas.</span><span class="sxs-lookup"><span data-stu-id="35bd3-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="35bd3-109">Se o dispositivo foi criptografado como resultado da configuração através da diretiva de grupo baseada em domínio, as informações de recuperação podem ser armazenadas no Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="35bd3-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

