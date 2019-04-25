---
title: Instalando o Office em um Terminal Server-não licenciado
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410110"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalando o Office em um Terminal Server

Para implantar o Office 365 proPlus em um servidor Windows usando serviços de área de trabalho remota (RDS), anteriormente denominado serviços de terminal:
  
- Você deve ter um plano do Office 365 que inclua o Office 365 proPlus, como o Office 365 Enterprise E3 ou Enterprise e5. Os planos do Office 365 Business e do Office 365 Business Premium não incluem o Office 365 proPlus.
    
- Você precisa habilitar a [ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Se você deseja instalar o Office 365 proPlus no RDS do portal do Office 365, * * *que usa as configurações de instalação padrão* * *, siga estas etapas: 
  
1. Verifique quais são os planos do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Se necessário, alterne para um plano diferente do Office 365. [Saiba como](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Se o Office já estiver instalado no servidor RDS usando qualquer outro plano do Office 365, desinstale-o. Por exemplo, indo para o painel \> de controle desinstalar um programa. DesInstale [o usando o assistente de recuperação e suporte da Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se você estiver executando problemas. 
    
4. No servidor RDS, entre no portal do Office 365 com sua conta de administrador e [Instale o Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Após a instalação do Office, * * *não abra ou entre* * * em qualquer aplicativo do Office. 
    
6. No servidor RDS, habilite a ativação de computador compartilhado editando o registro, seguindo estas etapas:
    
1. Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione executar. Na caixa abrir, digite **regedit**e, em seguida, selecione OK. 
    
2. Selecione Sim quando solicitado a permitir que o editor do Registro faça alterações em seu dispositivo.
    
3. No editor do registro, adicione um valor de cadeia de caracteres de **SharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. No servidor RDS, * * *entrar como um usuário final* * * e verificar se [a ativação de computador compartilhado está habilitada para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Para obter mais detalhes sobre os pré-requisitos, instruções de configuração e orientações sobre instalações personalizadas usando a ferramenta de implantação do Office, confira [implantar o office 365 ProPlus usando os serviços de área de trabalho remota](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Para corrigir erros relacionados à ativação de computador compartilhado, confira [solucionar problemas com a ativação de computador compartilhado para o Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

