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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807647"
---
# <a name="conditional-access-with-intune"></a>Acesso condicional com o Intune

O uso do  **acesso condicional**  com o Intune requer três etapas:

- Crie uma  **política de conformidade**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [Ios](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) para definir as configurações que devem ser atendidas antes que o dispositivo seja considerado compatível. Por exemplo, um dispositivo deve ter um PIN de pelo menos seis dígitos antes de ser considerado em conformidade.
- Criar uma **política de acesso condicional**  que define quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos.  [Por exemplo,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  um dispositivo deve estar em conformidade antes de acessar o email corporativo.
- Verifique se as políticas de **conformidade**  e  **as políticas de acesso condicional**  estão direcionadas para os grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários no Azure Active Directory.

**Links úteis:**

[Visão geral de conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Solucionando problemas de autoridade de certificação](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Política de solução de problemas](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Para proteger o email (Exchange Online) do acesso por dispositivos não compatíveis, ambos os documentos devem ser seguidos:

1. [Proteger o acesso de email de dispositivos usando EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteger o acesso de email de dispositivos usando clientes de autenticação modernos, como o Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)