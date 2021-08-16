---
title: Usando o Acesso Condicional com o Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005762"
---
# <a name="using-conditional-access-with-intune"></a>Usando o Acesso Condicional com o Intune

O uso do Acesso Condicional com o Intune requer três etapas:

- [Crie uma Política de Conformidade para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível. Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado compatível.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Crie uma Política de Acesso Condicional que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos. Por exemplo, um dispositivo deve estar em conformidade antes de acessar emails corporativos.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Verifique se as Políticas de Conformidade e as Políticas de Acesso Condicional são direcionadas aos grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Leia mais...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
