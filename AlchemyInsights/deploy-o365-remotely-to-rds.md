---
title: Implantando aplicativos do Microsoft 365 para empresas para uso compartilhado no RDS, Servidor de Terminal ou VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200661"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implantando aplicativos do Microsoft 365 para empresas para uso compartilhado no RDS, Servidor de Terminal ou VDI

Para implantar o Microsoft 365 Apps para empresas usando o RDS (Remote Desktop Services), anteriormente chamado de Serviços de Terminal:

- Você deve ter um plano do Microsoft 365 For Business ou um plano do Office 365 que inclua o Microsoft 365 Apps para empresas, como o Office 365 Enterprise E3 ou o Enterprise E5.
   > [!NOTE]
   > Os planos Microsoft 365 Apps for Business e Microsoft 365 Business Standard não incluem o Microsoft 365 Apps para empresas.
- Você deve [habilitar a ativação de computador compartilhado](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Você também pode baixar e executar o [Assistente de Recuperação](https://aka.ms/SaRA_OfficeSCA_M365Portal) e Suporte da Microsoft para instalar o Microsoft 365 Apps para empresas no modo de ativação de computador compartilhado.

Para obter mais informações sobre pré-requisitos, instruções de instalação e orientações sobre instalações personalizadas usando a Ferramenta de Implantação do Office, consulte [Deploy Microsoft 365 Apps for enterprise by](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)using Remote Desktop Services .

Para corrigir erros relacionados à ativação de computador compartilhado:

- Consulte [Solucionar problemas com a ativação de computador compartilhado para Aplicativos do Microsoft 365 para empresas.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Consulte [Redefina os aplicativos Microsoft 365 do estado de ativação empresarial](https://go.microsoft.com/fwlink/?linkid=2109218).

Se você quiser instalar o Microsoft 365 Apps para empresas no RDS do centro de administração do Microsoft 365, que usa configurações de instalação padrão, use as seguintes etapas:

1. Verifique qual assinatura você tem. [Saiba como](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Se necessário, alternar para uma assinatura diferente. [Saiba como](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Se o Office já estiver instalado no servidor RDS usando outras assinaturas da Microsoft, desinstale-o. Por exemplo, indo para **Painel de Controle**  >  **Desinstalar um programa**. Desinstalar [usando o Suporte e](https://aka.ms/SARA-OfficeUninstall-Alchemy) o Assistente de Recuperação da Microsoft se você estiver com problemas.
4. No servidor RDS, entre no Centro de administração do Microsoft 365 com sua conta de administrador e instale o [Microsoft 365 Apps para empresas.](https://portal.office.com/OLS/MySoftware.aspx)
5. Depois que o Office for instalado, ***não abra*** ou entre em nenhum aplicativo do Office.
6. No servidor RDS, habilita a ativação de computador compartilhado editando o Registro seguindo estas etapas:
   1. Clique com o botão direito do mouse no botão Windows no canto inferior esquerdo da tela e selecione **Executar**. Na caixa Abrir, digite **regedit** e selecione **OK**.
   2. Selecione **Sim** quando solicitado a permitir que o Editor do Registro faça alterações em seu dispositivo.
   3. No Editor do Registro, adicione um valor de cadeia de caracteres **sharedComputerLicensing** com uma configuração de 1 em HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. No servidor RDS, entre como usuário final e verifique se ***a*** ativação de computador compartilhado está habilitada para Aplicativos do [Microsoft 365 para empresas.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
