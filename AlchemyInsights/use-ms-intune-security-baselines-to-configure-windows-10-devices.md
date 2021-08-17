---
title: Usar Microsoft Intune de segurança para configurar Windows 10 dispositivos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104332"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Usar Microsoft Intune de segurança para configurar Windows 10 dispositivos

As linhas de base de segurança do Intune ajudam a proteger usuários e dispositivos. As linhas de base de segurança são grupos pré-configurados das configurações do Windows usados para aplicar um grupo conhecido de configurações e valores padrão recomendados por equipes de segurança relevantes. Ao criar um perfil de linha de base de segurança no Intune, você cria um modelo que consiste em vários perfis de configuração de dispositivo.

Quando você implanta linhas de base de segurança em grupos de usuários ou dispositivos, as configurações são aplicadas a dispositivos que são executados Windows 10 ou posteriores. Por exemplo, a Linha de Base de Segurança MDM automaticamente (1) habilita o BitLocker para unidades removíveis, (2) requer a senha para desbloquear um dispositivo e (3) desabilita a autenticação básica. Quando um valor padrão não funcionar para seu ambiente, personalize a linha de base para aplicar as configurações de que você precisa.

As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta no Microsoft 365. Veja a seguir alguns benefícios disso:

- Uma linha de base de segurança inclui as práticas recomendadas e recomendações para as configurações que afetam a segurança. Como os parceiros do Intune com a equipe de segurança do Windows que cria linhas de base para políticas de grupo, essas recomendações têm base em orientações sólidas e em uma vasta experiência.
- Se você não tiver certeza sobre onde começar no Intune, as linhas de base de segurança o ajudarão a criar e implantar rapidamente um perfil seguro.
- Se você usa atualmente uma política de grupo, migrar para o Intune para fins de gerenciamento é muito mais fácil com as linhas de base de segurança, pois elas são internas no Intune e incluem recursos de ponta para gerenciamento.

Para saber mais, consulte [Windows de segurança](https://go.microsoft.com/fwlink/?linkid=2141503) e gerenciamento de [dispositivos móveis.](https://go.microsoft.com/fwlink/?linkid=2141701)