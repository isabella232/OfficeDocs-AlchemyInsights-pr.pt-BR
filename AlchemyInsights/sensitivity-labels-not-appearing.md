---
title: Rótulos de sensibilidade que não aparecem
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061420"
---
# <a name="sensitivity-labels-not-appearing"></a>Rótulos de sensibilidade que não aparecem

Os rótulos de sensibilidade permitem que você classifique e ajude a proteger seu conteúdo confidenciais. Eles podem ser criados no centro de segurança Centro de conformidade do Microsoft 365, Microsoft 365 ou Microsoft 365 de segurança & Centro de Conformidade em Rótulos de > de Classificação. Para saber mais sobre esse recurso, consulte [Visão geral dos rótulos de sensibilidade.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Se você configurou seus rótulos de sensibilidade, mas eles não estão aparecendo nos aplicativos Microsoft 365, verifique o seguinte:

- Confirme se o rótulo de sensibilidade foi [publicado](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) para os usuários e grupos que você deseja.

- Confirme se o usuário está usando um aplicativo que dá suporte a rótulos de sensibilidade - consulte [rótulos de sensibilidade em seu documento](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Se você estiver migrando os rótulos da Proteção de Informações do [Azure,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)esteja ciente das considerações listadas [aqui](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Suporte à prevenção contra perda de dados (DLP): Atualmente, somente os rótulos de retenção podem ser usados como uma condição nas políticas de DLP.  O suporte para rótulos de sensibilidade em uma política de DLP ainda não está disponível, mas estamos trabalhando nele.

- Quando a criptografia é habilitada em um rótulo de sensibilidade, você pode escolher:
    - Atribuir permissões agora
    - Permitir que usuários atribuam permissões


Para obter mais informações sobre possíveis problemas, consulte [Problemas conhecidos com rótulos de sensibilidade.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)