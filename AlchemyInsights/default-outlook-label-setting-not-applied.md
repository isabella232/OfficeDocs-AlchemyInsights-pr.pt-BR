---
title: Configuração Outlook rótulo padrão não aplicada
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2021
ms.locfileid: "58370207"
---
# <a name="default-outlook-label-setting-not-applied"></a>Configuração Outlook rótulo padrão não aplicada

Se as configurações de rótulo padrão do seu Outlook não estão sendo aplicadas corretamente e um rótulo diferente ou nenhum rótulo é aplicado, você pode estar enfrentando um problema conhecido (MC277818) e deve fazer uma dessas duas opções para resolver o problema:

**Opção 1:**

1. Vá para o Microsoft 365 de Conformidade > **Proteção de Informações** de  >  **Soluções.**
1. Selecione **Políticas de** rótulo e selecione a política de rótulo que você precisa editar ( a configuração do **OutlookDefaultlabel** não está definida corretamente na política de rótulo em questão. Execute **Get-labelpolicy para** exibir essa configuração e selecione **Editar política**.
1. Selecione **Próximo** até ver a configuração Aplicar esse rótulo padrão aos **emails**, que estará disponível se  você selecionar Exigir que os usuários apliquem um rótulo **a emails** e documentos de herança na caixa de diálogo Configurações de Política.
1. Na caixa **de diálogo Aplicar um rótulo padrão** a documentos, escolha **Nenhum** na lista suspenso.
1. Selecione **Próximo** e **Enviar** para salvar suas configurações de rótulo.

**Opção 2:**

No [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)do Centro de Conformidade e Segurança, use o commandlet Set-LabelPolicy para alterar o **OutlookDefaultlabel** para **Nenhum** no {OutlookDefaultLabel="None"}.

Executar: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Para obter mais informações sobre rótulos padrão para Outlook, consulte [Definir um rótulo padrão diferente para Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).