---
title: Usar as linhas de base de segurança do Microsoft Intune para configurar dispositivos Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: 3bb93c196dd4717f5ec297e63284c5bc2840dcf5965cd000f336fde1e982a061
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971507"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Usar as linhas de base de segurança do Microsoft Intune para configurar dispositivos Windows 10

As linhas de base de segurança do Intune ajudam a proteger usuários e dispositivos. As linhas de base de segurança são grupos pré-configurados das configurações do Windows usados para aplicar um grupo conhecido de configurações e valores padrão recomendados por equipes de segurança relevantes. Ao criar um perfil de linha de base de segurança no Intune, você cria um modelo que consiste em vários perfis de configuração de dispositivo.

Quando você implanta linhas de base de segurança para grupos de usuários ou dispositivos, as configurações são aplicadas aos dispositivos que são executados no Windows 10 ou em versões posteriores. Por exemplo, a linha de base de segurança (1) de gerenciamento de dispositivo móvel da Microsoft (MDM) habilita o BitLocker para unidades removíveis, (2) requer a senha para desbloquear um dispositivo e (3) desabilita a autenticação básica. Quando um valor padrão não funciona para seu ambiente, você pode personalizar a linha de base para aplicar as configurações de que precisa.

As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta no Microsoft 365. Veja a seguir alguns benefícios dessa funcionalidade:
- Uma linha de base de segurança inclui as práticas recomendadas e recomendações para as configurações que afetam a segurança. Como os parceiros do Intune com a equipe de segurança do Windows que cria linhas de base para políticas de grupo, essas recomendações têm base em orientações sólidas e em uma vasta experiência.
- Se você não tiver certeza sobre onde começar no Intune, as linhas de base de segurança o ajudarão a criar e implantar rapidamente um perfil seguro.
- Se você estiver usando uma política de grupo no momento, migrar para o Intune para fins de gerenciamento é muito mais fácil com linhas de base de segurança, porque essas linhas de base de segurança são internas no Intune e incluem recursos de ponta para gerenciamento.

Para saber mais, consulte [as linhas de base de segurança do Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) e o [Gerenciamento de dispositivos móveis](https://docs.microsoft.com/windows/client-management/mdm/).