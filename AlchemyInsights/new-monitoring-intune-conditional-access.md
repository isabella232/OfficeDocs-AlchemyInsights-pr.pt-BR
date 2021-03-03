---
title: Monitorar o Acesso Condicional do Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416919"
---
# <a name="monitor-intune-conditional-access"></a>Monitorar o Acesso Condicional do Intune

Os usuários direcionados com acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:

1. Se presume-se que o dispositivo está inscrito, aconselha o usuário a ir até o aplicativo Portal da Empresa e verificar se ele aparece no Portal da Empresa. Se não for, o usuário deverá registrar o dispositivo.
1. No portal do Azure, vá para **Conformidade do Dispositivo do Intune.**  >   
1. Para exibir o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como **compatível,** em **Monitor,** clique em Conformidade do dispositivo.
1. No portal do Azure, vá para **Conformidade do Dispositivo do Intune.**  >   Em **Gerenciar,** clique em **Políticas**. Na lista de políticas de conformidade, verifique se um perfil está atribuído ao dispositivo do usuário. Se nenhum perfil for atribuído, o Intune não poderá confirmar o status de conformidade do dispositivo.
1. Edite a atribuição de acesso condicional do usuário.
1. No portal do Azure, navegue até Políticas de acesso condicional do **Intune,** selecione uma política na lista e clique em  >    >  Usuários **e grupos.**
1. Para direcionar uma determinada política para alguém, adicione-a à lista **Incluir**. Para garantir que uma pessoa seja omitida da política, adicione-a à lista **Excluir**.

**Links úteis:**

- [Visão geral da conformidade do dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Solução de problemas de CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Política de solução de problemas](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorando a conformidade do dispositivo do Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Essas etapas só são úteis na solução de problemas do recurso do Azure Active Directory Acesso Condicional. Também é possível colocar em quarentena um dispositivo bloqueando o acesso de email com a política do Exchange. Mais informações sobre o gerenciamento de dispositivos do Exchange podem ser encontradas [**aqui**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
