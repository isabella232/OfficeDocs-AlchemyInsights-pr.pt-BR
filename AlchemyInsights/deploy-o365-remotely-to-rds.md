---
title: Implantando o Microsoft 365 Apps for Enterprise para uso compartilhado no RDS, Terminal Server ou VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786265"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implantando o Microsoft 365 Apps for Enterprise para uso compartilhado no RDS, Terminal Server ou VDI

Para implantar o Microsoft 365 Apps for Enterprise usando serviços de área de trabalho remota (RDS), anteriormente denominado serviços de terminal:
- Você deve ter um plano do Microsoft 365 for Business ou um plano do Office 365 que inclua os aplicativos do Microsoft 365 para empresas, como o Office 365 Enterprise E3 ou Enterprise e5.
   > [!NOTE] 
   > Os planos padrão do Microsoft 365 Apps for Business e do Microsoft 365 Business Premium não incluem o Microsoft 365 aplicativos para empresas.
- Você deve habilitar a [ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Você também pode baixar e executar o [Assistente de recuperação e suporte da Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar o Microsoft 365 aplicativos para empresas no modo de ativação de computador compartilhado.

Para obter mais informações sobre pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, consulte [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Para corrigir erros relacionados à ativação de computador compartilhado:
- Consulte [solucionar problemas de ativação de computador compartilhado para o Microsoft 365 aplicativos para empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Consulte [Redefina os aplicativos Microsoft 365 do estado de ativação empresarial](https://go.microsoft.com/fwlink/?linkid=2109218).

Se você deseja instalar o Microsoft 365 aplicativos para empresas no RDS do centro de administração do Microsoft 365, ***que usa as configurações de instalação padrão***, use as seguintes etapas:

1.    Verifique a assinatura que você tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Se necessário, alterne para uma assinatura diferente. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Se o Office já estiver instalado no servidor RDS usando qualquer outra assinatura da Microsoft, desinstale-o. Por exemplo, indo para o **painel de controle**  >  **desinstalar um programa**. Desinstale [o usando o assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando problemas.
4.    No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e [Instale o Microsoft 365 aplicativos para empresas](https://portal.office.com/OLS/MySoftware.aspx).
5.    Após a instalação do Office, ***não abra ou entre*** em qualquer aplicativo do Office.
6.    No servidor RDS, habilite a ativação de computador compartilhado editando o registro, seguindo estas etapas:
   1. Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione **executar**. Na caixa abrir, digite **regedit**e, em seguida, selecione **OK**.
   2. Selecione **Sim** quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.
   3. No editor do registro, adicione um valor de cadeia de caracteres de **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. No servidor RDS, ***entre como um usuário final*** e verifique se [a ativação de computador compartilhado está habilitada para o Microsoft 365 aplicativos para empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

