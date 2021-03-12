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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708662"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorando o acesso condicional para o Exchange

Os usuários direcionados com acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:

- Se presume-se que o dispositivo está inscrito, aconselha o usuário a ir até o aplicativo Portal da Empresa e verificar se ele aparece no Portal da Empresa. Se não for, o usuário deverá registrar o dispositivo.
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

Observação: essas etapas só são úteis na solução de problemas do recurso do Azure Active Directory Acesso Condicional. Também é possível colocar em quarentena um dispositivo bloqueando o acesso de email com a política do Exchange. Mais informações sobre o gerenciamento de dispositivos do Exchange podem ser encontradas [aqui]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
