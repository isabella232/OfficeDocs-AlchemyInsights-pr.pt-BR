---
title: Usar Microsoft Intune de segurança para configurar Windows 10 dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331973"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Usar Microsoft Intune de segurança para configurar Windows 10 dispositivos

As linhas de base de segurança do Intune ajudam a proteger usuários e dispositivos. As linhas de base de segurança Windows configurações pré-configuradas usadas para aplicar um grupo conhecido de configurações e valores padrão recomendados pelas equipes de segurança relevantes. Ao criar um perfil de linha de base de segurança no Intune, você cria um modelo que consiste em vários perfis de configuração de dispositivo.

Quando você implanta linhas de base de segurança em grupos de usuários ou dispositivos, as configurações são aplicadas a dispositivos que são executados Windows 10 ou posteriores. Por exemplo, a linha de base de segurança de gerenciamento de dispositivo móvel (MDM) da Microsoft habilita automaticamente o BitLocker para unidades removíveis, exige a senha para desbloquear um dispositivo e desabilita a autenticação básica. Quando um valor padrão não funciona para seu ambiente, você pode personalizar a linha de base para aplicar as configurações de que precisa.

As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta no Microsoft 365. Uma linha de base de segurança inclui as práticas recomendadas e recomendações para as configurações que afetam a segurança. O Intune é parceiro da equipe de segurança Windows que cria linhas de base para políticas de grupo, portanto, essas recomendações se baseiam em orientações sólidas e em uma experiência extensa.

Se você for novo no Intune e não tiver certeza de onde começar, as linhas de base de segurança ajudarão você a criar e implantar rapidamente um perfil seguro. Se você usa atualmente uma política de grupo, migrar para o Intune para fins de gerenciamento é muito mais fácil com as linhas de base de segurança porque elas são internas no Intune e incluem recursos de gerenciamento de borda.

Para saber mais, consulte [Windows de segurança](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) e gerenciamento de [dispositivos móveis.](https://docs.microsoft.com/windows/client-management/mdm/)

