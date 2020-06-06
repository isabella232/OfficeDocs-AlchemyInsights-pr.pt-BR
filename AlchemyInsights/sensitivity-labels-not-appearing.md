---
title: Rótulos de sensibilidade não aparecem
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: df64022f6ad684e2af3eac080068536b7a167b74
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581003"
---
# <a name="sensitivity-labels-not-appearing"></a>Rótulos de sensibilidade não aparecem

Os rótulos de confidencialidade permitem classificar e ajudar a proteger o conteúdo confidencial. Eles podem ser criados no centro de conformidade da Microsoft 365, no centro de segurança da Microsoft 365 ou no centro de conformidade & segurança da Microsoft 365 em classificação > rótulos de confidencialidade. Para saber mais sobre esse recurso, confira [visão geral de rótulos de confidencialidade](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Se você configurou seus rótulos de sensibilidade, mas eles não estão aparecendo nos aplicativos do Microsoft 365, verifique o seguinte:

- Confirme se o rótulo de confidencialidade foi [publicado](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) nos usuários e grupos desejados.

- Confirme se o usuário está usando um aplicativo que oferece suporte a rótulos de confidencialidade-consulte [Rótulos de sensibilidade em seu documento](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Se você estiver [migrando os rótulos de proteção de informações do Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), esteja ciente das considerações listadas [aqui](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Suporte para prevenção de perda de dados (DLP): atualmente, somente rótulos de retenção podem ser usados como condição nas políticas de DLP.  O suporte para rótulos de confidencialidade em uma política de DLP ainda não está disponível, mas estamos trabalhando nele.

- Quando a criptografia estiver habilitada em um rótulo de confidencialidade, você poderá optar por:
    - Atribuir permissões agora
    - Permitir que usuários atribuam permissões


Para obter mais informações sobre possíveis problemas, consulte [problemas conhecidos com rótulos de confidencialidade](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).