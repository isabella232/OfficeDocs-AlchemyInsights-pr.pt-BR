---
title: Instalar o office em um servidor de Terminal - não licenciado
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274936"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalar o Office em um servidor de Terminal

Para implantar o Office 365 ProPlus em um servidor do Windows usando os serviços de área de trabalho remota (RDS), anteriormente conhecido como serviços de Terminal:
  
- Você deve ter um plano do Office 365 que inclui o Office 365 ProPlus, como o Office 365 Enterprise E3 ou E5 da empresa. Os planos de negócios do Office 365 e Office 365 Business Premium não incluem Office 365 ProPlus.
    
- Você precisará habilitar [a ativação do computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Se você deseja instalar o Office 365 ProPlus em RDS do portal do Office 365, * * *que usa as configurações de instalação padrão* * *, siga estas etapas: 
  
1. Verifique que você tem de plano do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Se necessário, alternar para um diferentes do Office 365 planejar. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Se o Office já estiver instalado no servidor RDS usando outros planos do Office 365, desinstale-o. Por exemplo, indo para painel de controle \> desinstalar um programa. Desinstale o usando o [Assistente de recuperação e de suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando nestes problemas. 
    
4. No servidor RDS, entre no portal do Office 365 com sua conta de administrador e [instalar o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Após a instalação do Office, * * *não abrir ou entrar* * * para quaisquer aplicativos do Office. 
    
6. No servidor RDS, habilite ativação do computador compartilhado por meio da edição do registro, seguindo estas etapas:
    
1. Com o botão direito no botão do Windows no canto inferior esquerdo da tela e selecione Executar. Na caixa Abrir, digite **regedit**e, em seguida, selecione Okey. 
    
2. Selecione Sim quando solicitado para permitir que o Editor do registro para fazer alterações em seu dispositivo.
    
3. No Editor do registro, adicione um valor de cadeia de caracteres do **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. No servidor RDS, * * *entrar como um usuário final* * * e [Verificar se a ativação do computador compartilhado está habilitada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Para obter mais detalhes sobre os pré-requisitos, instruções de instalação e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, consulte [Implantar o Office 365 ProPlus, usando os serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Para corrigir erros relacionados à ativação do computador compartilhado, consulte [Solucionar problemas com a ativação do computador compartilhado do Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

