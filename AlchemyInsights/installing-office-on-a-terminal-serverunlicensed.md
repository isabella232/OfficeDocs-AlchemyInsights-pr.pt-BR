---
title: Instalando o Office em um Terminal Server-não licenciado
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205397"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalando o Office em um Terminal Server

Para implantar o Office 365 ProPlus em um servidor Windows usando serviços de área de trabalho remota (RDS), anteriormente denominado serviços de terminal:
  
- Você deve ter um plano do Office 365 que inclua o Office 365 ProPlus, como o Office 365 Enterprise E3 ou Enterprise e5. Os planos do Office 365 Business e do Office 365 Business Premium não incluem o Office 365 ProPlus.

- Você precisa habilitar a [ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Se você deseja instalar o Office 365 ProPlus no RDS a partir do centro de administração do Microsoft 365, ***que usa as configurações de instalação padrão***, use as etapas a seguir.

> [!TIP]
> Você também pode baixar e executar o [Assistente de recuperação e suporte da Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar o Office 365 ProPlus no modo de ativação de computador compartilhado.
  
1. Verifique quais são os planos do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessário, alterne para um plano diferente do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Se o Office já estiver instalado no servidor RDS usando qualquer outro plano do Office 365, desinstale-o. Por exemplo, indo para o painel \> de controle desinstalar um programa. Desinstale [o usando o assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando problemas.

4. No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e [Instale o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Após a instalação do Office, ***não abra ou entre*** em qualquer aplicativo do Office.

6. No servidor RDS, habilite a ativação de computador compartilhado editando o registro, seguindo estas etapas:

1. Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione executar. Na caixa abrir, digite **regedit**e, em seguida, selecione OK.

2. Selecione Sim quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.

3. No editor do registro, adicione um valor de cadeia de caracteres de **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. No servidor RDS, ***entre como um usuário final*** e verifique se [a ativação de computador compartilhado está habilitada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Para obter mais detalhes sobre os pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, confira [implantar o office 365 ProPlus usando os serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Para corrigir erros relacionados à ativação de computador compartilhado, confira [solucionar problemas com a ativação de computador compartilhado para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  