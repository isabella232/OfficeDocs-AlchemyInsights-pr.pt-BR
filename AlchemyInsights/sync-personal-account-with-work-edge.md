---
title: Habilitar que um usuário sincronize uma conta pessoal com a conta de trabalho no Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: ad4b64c4bb50f50d4ab9fa47bb37228dce538e6d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317266"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Habilitar que um usuário sincronize uma conta pessoal com a conta de trabalho no Microsoft Edge

Certifique-se de atender a estes critérios:

- Enterprise State Roaming está habilitado no centro de administração do Azure Active Directory, o que requer uma assinatura para Azure Active Directory Premium ou Enterprise Mobility + Security (EMS). Para obter mais informações, [Enable Enterprise State Roaming em Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable).
- Um ou ambos os critérios a seguir são atendidos:
    - O serviço de Proteção de Informações do Azure está habilitado para o seu locatário. Para obter detalhes, consulte [Ativar a proteção do Azure Rights Management no centro de administração do Microsoft 365](https://docs.microsoft.com/azure/information-protection/activate-office365).
    - O recurso de Roaming de Estado da Empresa (ESR) do Azure Active Directory está habilitado para qualquer usuário ou locatário. Para obter mais informações, consulte [O que é o roaming de estado da empresa?](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview).

Se a AIP e o ESR estiverem desativados, uma mensagem de erro informará aos usuários que a sincronização não está disponível para as suas contas.
