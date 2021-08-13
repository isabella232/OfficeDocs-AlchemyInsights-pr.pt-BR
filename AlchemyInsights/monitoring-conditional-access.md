---
title: Monitoramento do Acesso Condicional
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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975089"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorando o acesso condicional para Exchange

Os usuários direcionados com acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:

- Se presume-se que o dispositivo está inscrito, informe o usuário a ir até o aplicativo Portal da Empresa e verifique se ele aparece no Portal da Empresa. Se não for, o usuário deverá registrar o dispositivo.
- No portal do Azure, acesse Intune > Conformidade com o dispositivo. Em Monitorar, clique em Conformidade com o dispositivo. Exibir o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como compatível.
- No portal do Azure, acesse Intune > Conformidade com o dispositivo. Em Gerenciar, clique em Políticas. Na lista de políticas de conformidade, verifique se um perfil está atribuído ao dispositivo do usuário. Se nenhum perfil for atribuído, o Intune não poderá confirmar o status de conformidade do dispositivo.
- Edite a atribuição de acesso condicional do usuário.

1. No portal do Azure, acesse Políticas de acesso condicional do **Intune.**  >    >  
2. Selecione uma política na lista.
3. Clique em Usuários e grupos.
4. Para direcionar uma determinada política para alguém, adicione-a à lista Incluir. Para garantir que uma pessoa seja omitida da política, adicione-a à lista Excluir.

Links úteis:

[Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Solução de problemas de CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Política de solução de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorando a conformidade do dispositivo do Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Observação: essas etapas só são úteis na solução de problemas do recurso Azure Active Directory Acesso Condicional. Também é possível colocar em quarentena um dispositivo bloqueando o acesso de email com Exchange política. Mais informações sobre Exchange gerenciamento de dispositivos podem ser encontradas [aqui]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
