---
title: Implantando Teams como autônomo ou com instalações novas ou Office existentes
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320110"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implantando Teams como autônomo ou com instalações novas ou Office existentes

Microsoft Teams agora está incluído como  parte de novas instalações de Microsoft 365 Apps para Grandes Empresas, Microsoft 365 Apps para Pequenos e Médios negócios e Office para Mac. Para mais informações, confira [Quando o Microsoft Teams começará a ser incluído nas novas instalações do Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Além disso, a partir da versão 1906 no Canal Atual, o Teams será adicionado às instalações existentes do Microsoft 365 Apps para Grandes Empresas (e Microsoft 365 Apps para Pequenos e Médios negócios) em ***dispositivos*** que executam o Windows quando você atualizar sua instalação existente para a versão mais recente. Para mais informações, confira [E as instalações existentes do Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Observação:** se você não quiser esperar por essa agenda de lançamento, poderá implantar o Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) como autônomo para seus usuários seguindo essas instruções ou pode fazer com que seus usuários instalem o Teams para si mesmos a partir de [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Se sua organização não estiver pronta para implantar Teams, temos as etapas que você [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) pode [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) seguir para excluir Teams instalações novas ou existentes de Office.  Se você quiser que o Teams seja instalado, mas que não seja iniciado automaticamente para o usuário após a instalação, confira [Impedir que o Microsoft Teams seja iniciado automaticamente após a instalação](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Para ***desinstalar o Teams*** de um dispositivo com Windows, confira [Desinstalar o Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Para limpar o Microsoft Teams de vários usuários ou máquinas de destino, [consulte Microsoft Teams implantação de limpeza](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Se você estiver usando computadores compartilhados, Serviços de Área de Trabalho Remota (RDS) ou VDI (Virtual Desktop Infrastructure), confira [Computadores compartilhados e ambientes de VDI com o Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Se você estiver usando o Office para Mac, confira [Instalações do Microsoft Teams em um Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Observação**: após Teams instalado, ele [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) é atualizado automaticamente aproximadamente a cada duas semanas com novos recursos e atualizações de qualidade. 