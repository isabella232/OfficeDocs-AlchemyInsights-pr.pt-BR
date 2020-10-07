---
title: Monitorar o acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366416"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorar o acesso condicional do Exchange

Os usuários direcionados ao acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:

- Se presumir que o dispositivo esteja inscrito, recomende que o usuário acesse o aplicativo do portal da empresa e verifique se ele aparece no portal da empresa. Caso contrário, o usuário deverá registrar o dispositivo.
- No portal do Azure, acesse o Intune > o dispositivo de conformidade. Em monitorar, clique em conformidade de dispositivo. Exiba o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como compatível.
- No portal do Azure, acesse o Intune > o dispositivo de conformidade. Em gerenciar, clique em políticas. Na lista de políticas de conformidade, verifique se um perfil foi atribuído ao dispositivo do usuário. Se nenhum perfil for atribuído, o Intune não conseguirá confirmar o status de conformidade do dispositivo.
- Edite a atribuição de acesso condicional do usuário.

1. No portal do Azure, acesse **Intune**  >  **Conditional access**  >  **as políticas**de acesso condicional do Intune.
2. Selecione uma política na lista.
3. Clique em usuários e grupos.
4. Para direcionar uma determinada política em alguém, adicione-a à lista de inclusões. Para garantir que uma pessoa seja omitida da política, adicione-a à lista de exclusão.

Links úteis:

[Visão geral de conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Solucionando problemas de autoridade de certificação](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Política de solução de problemas](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Monitoramento da conformidade do dispositivo do Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Observação: estas etapas só são úteis para solucionar problemas de acesso condicional ao recurso do Azure Active Directory. Também é possível colocar em quarentena um dispositivo que bloqueie o acesso de email com a política do Exchange. Mais informações sobre o gerenciamento de dispositivos do Exchange podem ser encontradas [aqui](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
