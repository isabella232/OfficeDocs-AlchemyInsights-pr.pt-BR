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
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025490"
---
# <a name="monitor-intune-conditional-access"></a>Monitorar o Acesso Condicional do Intune

Os usuários direcionados com acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:

1. Se presume-se que o dispositivo está inscrito, informe o usuário a ir até o aplicativo Portal da Empresa e verifique se ele aparece no Portal da Empresa. Se não for, o usuário deverá registrar o dispositivo.
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
> Essas etapas só são úteis na solução de problemas do recurso Azure Active Directory Acesso Condicional. Também é possível colocar em quarentena um dispositivo bloqueando o acesso de email com Exchange política. Mais informações sobre o Exchange gerenciamento de dispositivos podem ser encontradas [**aqui**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
