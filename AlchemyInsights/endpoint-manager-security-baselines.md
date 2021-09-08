---
title: EndPoint Manager - Linhas de base de segurança
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923542"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Linhas de base de segurança

As linhas de base de segurança são grupos pré-configurados de configurações do Windows que ajudam você a aplicar as configurações de segurança recomendadas pelas equipes de segurança relevantes. Essas linhas de base podem ser personalizadas para entregar apenas as configurações e valores desejados. Para mais informações sobre linhas de base de segurança, consulte [Utilizar linhas de base de segurança para configurar dispositivos Windows 10 no Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Existem atualmente linhas de base para esses produtos:

- Configurações de segurança do Windows MDM
- Segurança do Microsoft Defender para Ponto de Extremidade
- Microsoft Edge

Cada uma das linhas de base são atualizadas periodicamente e lançadas em versões incrementais. Cada versão adiciona e remove as configurações da versão anterior para garantir que a linha de base atenda às orientações atuais. O console de linhas de base de Segurança na Segurança do Ponto de extremidade permite que diferentes versões sejam comparadas, tornando visíveis as mudanças de versão para versão.

Para orientações sobre como alterar, com mais eficácia, qual versão da linha de base será implantada, consulte [Gerenciar perfis de linha de base de segurança no Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Após a implantação de uma linha de base de segurança, você pode monitorar o estado da implantação e analisar as configurações com base em cada dispositivo.

Como as linhas de base de segurança contêm muitas configurações, é importante rever as alterações de configuração e executar testes para garantir que todas as configurações sejam apropriadas para seus dispositivos e necessidades de negócios.

**Observação:** Os dados de relatórios para linhas de base podem levar até 24 horas para aparecer a partir da implantação inicial para um dispositivo e até 6 horas para novas atualizações. 

A causa mais comum da não aplicação de uma configuração de base é porque a mesma configuração está sendo utilizada em um perfil diferente. Este cenário pode ser investigado para um dispositivo específico, selecionando esse dispositivo dentro do nó de Status do Dispositivo do perfil da Linha de Base de Segurança. Para maiores detalhes, consulte [Resolver conflitos para linhas de base de segurança](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).