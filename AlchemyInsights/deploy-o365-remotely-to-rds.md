---
title: Implantando Microsoft 365 Apps para Grandes Empresas para uso compartilhado no RDS, Servidor de Terminal ou VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60040994"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implantando Microsoft 365 Apps para Grandes Empresas para uso compartilhado no RDS, Servidor de Terminal ou VDI

Para implantar Microsoft 365 Apps serviços de área de trabalho remota (RDS), anteriormente Serviços de Terminal, você deve:

- Use a correção fácil para habilitar o TLS 1.2 como padrão se você estiver executando uma versão mais antiga do Windows (por exemplo, Windows 7 SP1, Windows Server 2008 R2). Para obter uma correção fácil e mais informações, consulte [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy). 
- Tenha um plano que inclua Microsoft 365 Apps para Grandes Empresas (anteriormente Office 365 Plus). Por exemplo, Office 365 E3 ou Microsoft 365 E5, ou qualquer plano que inclua a versão da área de trabalho do Project ou Visio, como Project Plano 3 ou Visio Plano 2, ou o plano Microsoft 365 Business Premium, que também inclui Microsoft 365 Apps para Pequenos e Médios negócios.
- Habilitar a ativação de computador compartilhado. Para obter mais informações, consulte [Overview of shared computer activation for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Observação**: para instalar Microsoft 365 Apps no modo de ativação de computador compartilhado, baixe e execute o [microsoft Assistente de Recuperação e Suporte](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds). Para obter detalhes sobre pré-requisitos, instruções de instalação e orientações para personalizar instalações usando a Ferramenta de Implantação Office, consulte [Deploy Microsoft 365 Apps by using Remote Desktop Services](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Para corrigir erros relacionados à ativação de computador compartilhado, consulte:

- [Solucionar problemas com a ativação de computador compartilhado para Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Redefinir os Aplicativos do Microsoft 365 para o estado de ativação empresarial](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Se você quiser instalar o Microsoft 365 Apps no RDS do Centro de administração do Microsoft 365, que usa as configurações de instalação padrão, siga estas etapas:

1. Verifique o Microsoft 365 plano que você tem. Para obter mais informações, consulte [Qual assinatura eu tenho?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Se necessário, alternar para um plano Microsoft 365 diferente. Para obter mais informações, [consulte Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Se Microsoft 365 Apps já estiver instalado no servidor RDS usando quaisquer outros planos incompatíveis, desinstale-o indo para **Painel** de Controle  >  **Desinstalar um programa**. Se você tiver problemas, desinstale baixando [o Microsoft Assistente de Recuperação e Suporte](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. No servidor RDS, entre no Centro de administração do Microsoft 365 com sua conta de administrador e [instale Office](https://portal.office.com/OLS/MySoftware.aspx).

   Depois Office estiver instalado, não abra ou entre em nenhum Office aplicativos.

1. No servidor RDS, habilita a ativação de computador compartilhado editando o Registro:

   1. Clique com o botão direito do Windows no canto inferior esquerdo da tela e selecione **Executar**. Na caixa Abrir, digite **regedit** e selecione **OK**.

   1. Quando solicitado a permitir que o Editor do Registro faça alterações em seu dispositivo, selecione **Sim**.

   1. No Editor do Registro, em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, adicione um valor de cadeia de caracteres **de SharedComputerLicensing** com uma configuração **de 1** .

1. No servidor RDS, entre como usuário final e verifique se a ativação de computador compartilhado está habilitada para Microsoft 365 Apps. 

   Para obter detalhes, [consulte Verify that shared computer activation is enabled for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).