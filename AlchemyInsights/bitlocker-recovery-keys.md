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
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060052"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Acessando chaves de recuperação do Bitlocker

Ao configurar configurações do Bitlocker Notune Endpoint Protection Política, é possível definir se as informações de recuperação do Bitlocker devem ser armazenadas em Azure Active Directory.

Se essa configuração estiver configurada, os dados de recuperação armazenados devem estar visíveis para um administrador do Intune como parte dos dados de registro do dispositivo na folha Dispositivos do Intune de duas maneiras:

Dispositivos - dispositivos do Azure AD -> "Device" OR Devices -> All Devices -> "Device" -> Recovery keys

Como alternativa, se houver acesso administrativo ao dispositivo em si, a chave de recuperação (Senha) poderá ser vista executando o seguinte comando de um prompt de comando elevado:

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
Se o dispositivo foi criptografado antes da inscrição no Intune, a chave de recuperação pode ter sido associada à "Conta da Microsoft" (MSA) usada para entrar no dispositivo durante o processo OOBE. Se esse for o caso, acessar e entrar com esse MSA deve mostrar os dispositivos para os quais as chaves  https://onedrive.live.com/recoverykey de recuperação foram armazenadas.
 
Se o dispositivo foi criptografado como resultado da configuração por meio de política de grupo baseada em domínio, as informações de recuperação poderão ser armazenadas no Active Directory local.

Se você configurou a política de proteção de ponto de extremidade para armazenar a chave de recuperação no Azure Active Directory, mas a chave de um dispositivo específico não foi carregada, você pode disparar o carregamento girando a chave de recuperação para esse dispositivo do console MEM. Para obter detalhes, consulte [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

