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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508616"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalando o Office em um Terminal Server

Para implantar o Microsoft 365 aplicativos para empresas em um servidor Windows usando serviços de área de trabalho remota (RDS), anteriormente denominado serviços de terminal:
  
- Você deve ter uma assinatura do Microsoft 365 que inclui aplicativos da Microsoft 365 para empresas, como o Office 365 Enterprise E3 ou Enterprise e5. Os planos Microsoft 365 Apps for Business e Microsoft 365 aplicativos para Business Premium não incluem o Microsoft 365 aplicativos para empresas.

- Você precisa habilitar a [ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Se você deseja instalar o Microsoft 365 aplicativos para empresas no RDS do centro de administração do Microsoft 365, ***que usa as configurações de instalação padrão***, use as etapas a seguir.

> [!TIP]
> Você também pode baixar e executar o [Assistente de recuperação e suporte da Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar o Microsoft 365 aplicativos para empresas no modo de ativação de computador compartilhado.
  
1. Verifique a assinatura do Microsoft 365 que você tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessário, alterne para uma assinatura do Microsoft 365 diferente. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Se o Office já estiver instalado no servidor RDS usando qualquer outra assinatura do Microsoft 365, desinstale-o. Por exemplo, indo para o painel de controle \> desinstalar um programa. Desinstale [o usando o assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando problemas.

4. No servidor RDS, entre no centro de administração do Microsoft 365 com sua conta de administrador e [Instale o Microsoft 365 aplicativos para empresas](https://portal.office.com/OLS/MySoftware.aspx).

5. Após a instalação do Office, ***não abra ou entre*** em qualquer aplicativo do Office.

6. No servidor RDS, habilite a ativação de computador compartilhado editando o registro, seguindo estas etapas:

1. Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione executar. Na caixa abrir, digite **regedit**e, em seguida, selecione OK.

2. Selecione Sim quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.

3. No editor do registro, adicione um valor de cadeia de caracteres de **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. No servidor RDS, ***entre como um usuário final*** e verifique se [a ativação de computador compartilhado está habilitada para o Microsoft 365 aplicativos para empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Para obter mais detalhes sobre os pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, consulte [implantar o Microsoft 365 Apps for Enterprise usando serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Para corrigir erros relacionados à ativação de computador compartilhado, confira [solucionar problemas com a ativação de computador compartilhado para o Microsoft 365 Apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  