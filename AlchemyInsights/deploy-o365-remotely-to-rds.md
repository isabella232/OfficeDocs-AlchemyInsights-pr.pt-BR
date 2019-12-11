---
title: Implantando o Office 365 PROPLUS para uso compartilhado no RDS, no Terminal Server ou no VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959448"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implantando o Office 365 PROPLUS para uso compartilhado no RDS, no Terminal Server ou no VDI

Para implantar o Office 365 ProPlus usando os serviços de área de trabalho remota (RDS), anteriormente denominado serviços de terminal:
- Você deve ter um plano do Microsoft 365 para empresas ou um plano do Office 365 que inclua o Office 365 ProPlus, como o Office 365 Enterprise E3 ou Enterprise e5.
   > [!NOTE] 
   > Os planos do Office 365 Business e do Office 365 Business Premium não incluem o Office 365 ProPlus.
- Você deve habilitar a [ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Você também pode baixar e executar o [Assistente de recuperação e suporte da Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar o Office 365 ProPlus no modo de ativação de computador compartilhado.

Para obter mais informações sobre pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, confira [implantar o office 365 ProPlus usando os serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Para corrigir erros relacionados à ativação de computador compartilhado:
- Consulte [solucionar problemas de ativação de computador compartilhado para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Consulte [Reset Office 365 ProPlus Activation State](https://go.microsoft.com/fwlink/?linkid=2109218).

Se você deseja instalar o Office 365 ProPlus no RDS a partir do centro de administração do Microsoft 365, ***que usa as configurações de instalação padrão***, use as seguintes etapas:

1.  Verifique quais são os planos do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Se necessário, alterne para um plano diferente do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Se o Office já estiver instalado no servidor RDS usando qualquer outro plano do Office 365, desinstale-o. Por exemplo, indo para o **painel** > de controle**desinstalar um programa**. Desinstale [o usando o assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando problemas.
4.  No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e [Instale o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Após a instalação do Office, ***não abra ou entre*** em qualquer aplicativo do Office.
6.  No servidor RDS, habilite a ativação de computador compartilhado editando o registro, seguindo estas etapas:
   1. Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione **executar**. Na caixa abrir, digite **regedit**e, em seguida, selecione **OK**.
   2. Selecione **Sim** quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.
   3. No editor do registro, adicione um valor de cadeia de caracteres de **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. No servidor RDS, ***entre como um usuário final*** e verifique se [a ativação de computador compartilhado está habilitada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

