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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325591"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implantando Microsoft 365 Apps para Grandes Empresas para uso compartilhado no RDS, Servidor de Terminal ou VDI

Para implantar Microsoft 365 Apps para Grandes Empresas serviços de área de trabalho remota (RDS), anteriormente denominados Serviços de Terminal:

- Você deve ter um plano Microsoft 365 para Empresas ou um plano Office 365 que inclua Microsoft 365 Apps para Grandes Empresas, como Office 365 Enterprise E3 ou Enterprise E5.
   **Observação**: os Microsoft 365 Apps para Pequenos e Médios negócios e Microsoft 365 Business Standard não incluem Microsoft 365 Apps para Grandes Empresas.
- Você deve [habilitar a ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

**Observação**: você também pode baixar e executar o [microsoft Assistente de Recuperação e Suporte](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar Microsoft 365 Apps para Grandes Empresas no modo de ativação de computador compartilhado.

Para obter mais informações sobre pré-requisitos, instruções de instalação e orientações sobre instalações personalizadas usando Office Ferramenta de Implantação do Office, consulte [Deploy Microsoft 365 Apps para Grandes Empresas by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Para corrigir erros relacionados à ativação de computador compartilhado:

- Consulte [Solucionar problemas com a ativação de computador compartilhado para Microsoft 365 Apps para Grandes Empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Consulte [Redefina os aplicativos Microsoft 365 do estado de ativação empresarial](https://go.microsoft.com/fwlink/?linkid=2109218).

Se você quiser instalar o Microsoft 365 Apps para Grandes Empresas no RDS do ***Centro de administração do Microsoft 365,*** que usa as configurações de instalação padrão, use as seguintes etapas:

1. Verifique qual assinatura você tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Se necessário, alternar para uma assinatura diferente. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Se Office já estiver instalado no servidor RDS usando qualquer outra assinatura da Microsoft, desinstale-a. Por exemplo, indo para **Painel de Controle**  >  **Desinstalar um programa**. Desinstalar [usando Assistente de Recuperação e Suporte](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft se você estiver com problemas.
4. No servidor RDS, entre no Centro de administração do Microsoft 365 com sua conta de administrador e [instale Microsoft 365 Apps para Grandes Empresas](https://portal.office.com/OLS/MySoftware.aspx).
5. Depois Office estiver instalado, ***não abra*** ou entre em nenhum Office aplicativos.
6. No servidor RDS, habilita a ativação de computador compartilhado editando o Registro seguindo estas etapas:
   1. Clique com o botão direito do Windows no canto inferior esquerdo da tela e selecione **Executar**. Na caixa Abrir, digite **regedit** e selecione **OK**.
   2. Selecione **Sim** quando solicitado a permitir que o Editor do Registro faça alterações em seu dispositivo.
   3. No Editor do Registro, adicione um valor de cadeia de caracteres **sharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. No servidor RDS, entre como usuário final e verifique se ***a*** ativação de computador compartilhado está habilitada [para](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)Microsoft 365 Apps para Grandes Empresas .
