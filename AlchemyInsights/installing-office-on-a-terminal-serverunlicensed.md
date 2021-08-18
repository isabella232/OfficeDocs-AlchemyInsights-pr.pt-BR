---
title: Instalando o office em um Servidor de Terminal - Sem licença
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321987"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalando Office em um Servidor de Terminal

Para implantar o Microsoft 365 Apps para Grandes Empresas em um servidor Windows usando o RDS (Remote Desktop Services), anteriormente chamado de Serviços de Terminal:
  
- Você deve ter uma assinatura Microsoft 365 que inclua Microsoft 365 Apps para Grandes Empresas, como Office 365 Enterprise E3 ou Enterprise E5. Os Microsoft 365 Apps para Pequenos e Médios negócios e Microsoft 365 Apps para Pequenos e Médios negócios Premium não incluem Microsoft 365 Apps para Grandes Empresas.

- Você precisa habilitar a [ativação de computador compartilhado.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Se você quiser instalar o Microsoft 365 Apps para Grandes Empresas no RDS do ***Centro de administração do Microsoft 365,*** que usa as configurações de instalação padrão, use as etapas a seguir.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Verifique o Microsoft 365 assinatura que você tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Se necessário, alternar para uma assinatura Microsoft 365 diferente. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Se Office já estiver instalado no servidor RDS usando qualquer outra assinatura Microsoft 365, desinstale-a. Por exemplo, indo para Painel de Controle \> Desinstalar um programa. Desinstalar [usando Assistente de Recuperação e Suporte](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft se você estiver com problemas.

4. No servidor RDS, entre no Centro de administração do Microsoft 365 com sua conta de administrador e [instale Microsoft 365 Apps para Grandes Empresas](https://portal.office.com/OLS/MySoftware.aspx).

5. Depois Office estiver instalado, ***não abra*** ou entre em nenhum Office aplicativos.

6. No servidor RDS, habilita a ativação de computador compartilhado editando o Registro seguindo estas etapas:

1. Clique com o botão direito do Windows no canto inferior esquerdo da tela e selecione Executar. Na caixa Abrir, digite **regedit** e selecione OK.

2. Selecione Sim quando solicitado a permitir que o Editor do Registro faça alterações em seu dispositivo.

3. No Editor do Registro, adicione um valor de cadeia de caracteres **sharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. No servidor RDS, entre como usuário final e verifique se ***a*** ativação de computador compartilhado está habilitada [para](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)Microsoft 365 Apps para Grandes Empresas .

Para obter mais detalhes sobre os pré-requisitos, instruções de instalação e orientações sobre instalações personalizadas usando Office Ferramenta de Implantação do Office, consulte [Deploy Microsoft 365 Apps para Grandes Empresas by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Para corrigir erros relacionados à ativação de computador compartilhado, consulte Solucionar problemas com a ativação de computador [compartilhado para Microsoft 365 Apps para Grandes Empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  