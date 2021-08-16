---
title: Acesso condicional com o Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069700"
---
# <a name="conditional-access-with-intune"></a>Acesso condicional com o Intune

O uso  **do Acesso Condicional**  com o Intune requer três etapas:

- Crie uma **Política de Conformidade** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível. Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado compatível.
- Crie uma **Política de Acesso Condicional**  que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos.  [Por exemplo, um](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  dispositivo deve estar em conformidade antes de acessar emails corporativos.
- Verifique se **as Políticas de Conformidade**  e as Políticas de Acesso  **Condicional**  são direcionadas aos grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários Azure Active Directory.

**Links úteis:**

[Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Solução de problemas de CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Política de solução de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Para proteger Email (Exchange online) do acesso por dispositivos não compatíveis, ambos os documentos devem ser seguidos:

1. [Proteger o acesso de email contra dispositivos usando o EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteger o acesso de email contra dispositivos que usam clientes de autenticação modernos, como Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)