---
title: Usar as linhas de base de segurança do Microsoft Intune para configurar dispositivos Windows 10
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571765"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Usar as linhas de base de segurança do Microsoft Intune para configurar dispositivos Windows 10

As linhas de base de segurança do Intune ajudam a proteger usuários e dispositivos. As linhas de base de segurança são os grupos pré-configurados de configurações do Windows usados para aplicar um grupo conhecido de configurações e valores padrão recomendados pelas equipes de segurança relevantes. Ao criar um perfil de linha de base de segurança no Intune, você cria um modelo que consiste em vários perfis de configuração de dispositivo.

Quando você implanta linhas de base de segurança para grupos de usuários ou dispositivos, as configurações são aplicadas a dispositivos executados no Windows 10 ou posterior. Por exemplo, a linha de base de segurança MDM automaticamente (1) habilita o BitLocker para unidades removíveis, (2) requer a senha para desbloquear um dispositivo e (3) desabilita a autenticação básica. Quando um valor padrão não funciona para seu ambiente, personalize a linha de base para aplicar as configurações de que você precisa.

As linhas de base de segurança também ajudam a estabelecer um fluxo de trabalho seguro de ponta a ponta no Microsoft 365. Estes são alguns dos benefícios disso:

- Uma linha de base de segurança inclui as práticas recomendadas e as recomendações para as configurações que afetam a segurança. Como os parceiros do Intune com a equipe de segurança do Windows que cria linhas de base para diretivas de grupo, essas recomendações são baseadas em uma orientação sólida e uma ampla experiência.
- Se você é novo no Intune e não tem certeza de onde começar, as linhas de base de segurança ajudarão você a criar e implantar rapidamente um perfil seguro.
- Se você usa uma política de grupo no momento, a migração para o Intune para fins de gerenciamento é muito mais fácil com as linhas de base de segurança, pois elas são criadas no Intune e incluem recursos de recorte de borda para gerenciamento.

Para saber mais, confira [Windows Security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile Device Management](https://go.microsoft.com/fwlink/?linkid=2141701).