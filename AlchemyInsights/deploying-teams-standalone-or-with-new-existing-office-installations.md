---
title: Implantando o Microsoft Teams como autônomo ou com instalações do Office novas ou existentes
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806747"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implantando o Microsoft Teams como autônomo ou com instalações do Office novas ou existentes

O Microsoft Teams agora está incluído como parte de ***novas instalações*** do Microsoft 365 aplicativos para empresas, aplicativos do Microsoft 365 para empresas e Office para Mac. Para mais informações, confira [Quando o Microsoft Teams começará a ser incluído nas novas instalações do Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Além disso, a partir da versão 1906 no canal atual, as equipes serão ***adicionadas às instalações existentes*** dos aplicativos da Microsoft 365 para empresas (e aplicativos do Microsoft 365 para empresas) em dispositivos que executam o Windows quando você atualiza sua instalação existente para a versão mais recente. Para mais informações, confira [E as instalações existentes do Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Se não quiser aguardar esse cronograma de distribuição, você pode implantar o Microsoft Teams como autônomo para seus usuários [seguindo estas instruções](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ou pode fazer com que seus usuários instalem o Teams por conta própria  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Se sua organização não estiver pronta para implantar o Teams, temos as etapas que você pode executar para ***excluir equipes*** de instalações [novas](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ou [existentes](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) do Office. Se você quiser que o Teams seja instalado, mas que não seja iniciado automaticamente para o usuário após a instalação, confira [Impedir que o Microsoft Teams seja iniciado automaticamente após a instalação](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Para ***desinstalar o Teams*** de um dispositivo com Windows, confira [Desinstalar o Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Para limpar o Microsoft Teams de várias máquinas de destino ou usuários, confira [implantação do Microsoft Teams Clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Se você estiver usando computadores compartilhados, Serviços de Área de Trabalho Remota (RDS) ou VDI (Virtual Desktop Infrastructure), confira [Computadores compartilhados e ambientes de VDI com o Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Se você estiver usando o Office para Mac, confira [Instalações do Microsoft Teams em um Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Depois que o Microsoft Teams é instalado, ele é [atualizado automaticamente](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) aproximadamente a cada duas semanas com novos recursos e atualizações de qualidade. 