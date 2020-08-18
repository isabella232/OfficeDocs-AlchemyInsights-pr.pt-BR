---
title: Alterar canais de atualização de Aplicativos do Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 43a3cdefe5a9bc1726984a3195dce7aaea08d892
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786841"
---
# <a name="change-update-channels-for-office-apps"></a>Alterar canais de atualização de Aplicativos do Office

Para novas instalações do Office, use as Configurações de Download de Software do Office para escolher o canal de atualização e, em seguida, instale (ou reinstale) os aplicativos do Office. Para saber mais, veja [Gerenciar as Configurações de Download de Software no Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Observação** o canal de atualização selecionado usando as Configurações de Download de Software do Office se aplica a todos os usuários executando novas instalações usando o portal do O365. Para saber mais informações, confira [Baixar e instalar ou reinstalar o Microsoft 365 ou o Office 2019 em PC ou Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Para instalações existentes do Office, use a Ferramenta de Implantação do Office (ODT) para mudar para outro um canal de atualização:  

1. Baixe a versão mais recente da Ferramenta de Implantação do Office (setup.exe) no [Centro de Download da Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identifique o nome do canal para o qual você deseja mudar. Para saber mais informações, veja [Opções de configuração da Ferramenta de Implantação do Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Crie um arquivo XML de configuração especificando o nome do canal apropriado, por exemplo, update.xml.  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. Em um prompt de comando elevado, alterne para o local da pasta do setup.exe e execute o seguinte comando:  
    a. setup.exe /configure update.xml
5. Inicie um aplicativo do Office (como o Excel) e, em seguida, selecione **Arquivo** > **Conta**. Na seção Informações do Produto, selecione **Opções de Atualização** > **Atualizar Agora**.

Para saber mais, veja [Como alternar canais de atualização de aplicativos existentes do Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Para alternar os canais de atualização de um grupo de usuários selecionado ou usando o Configuration Manager (SCCM), defina a configuração do Canal de Atualização usando o GPO. Para obter mais informações, confira [Visão geral dos canais de atualização do Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Para obter detalhes, confira [Como gerenciar canais do Office 365 ProPlus para profissionais de TI](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) e [Gerenciar atualizações do Microsoft 365 Apps com o Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).