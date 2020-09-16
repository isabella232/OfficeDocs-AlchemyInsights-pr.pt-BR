---
title: Controlar atualizações automáticas de Aplicativos do Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747764"
---
# <a name="control-automatic-updates-for-office-apps"></a>Controlar atualizações automáticas de Aplicativos do Office

Por padrão, atualizações de Aplicativos do Office são baixadas e aplicadas automaticamente em segundo plano, sem nenhuma intervenção do usuário. No entanto, os administradores podem controlar como as atualizações são aplicadas usando as configurações de Atualização do Office. As configurações de atualização permitem aos administradores habilitar ou desabilitar atualizações automáticas, mostrar ou ocultar o botão **Atualizar agora** no Office, definir prazos de atualização e muito mais. Para obter informações detalhadas, veja:

- [Configurar definições de atualização do Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Atualização automática do Office não está habilitada](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definir como o Office será atualizado após sua instalação](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Para analisar as configurações de atualizações existentes aplicadas a um computador cliente, siga estas etapas:

1. Abra o Editor do Registro acessando **Iniciar** > **Executar** > **regedit**.
2. Mude para o local a seguir e analise as configurações de Atualização do Office:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Observação** se a chave OfficeMgmtCOM estiver definida, você poderá ver a mensagem "Atualizações são gerenciadas pelo administrador do sistema" em **Office** > **Conta** > **Atualizações do Office**. Para saber mais, confira [Gerenciar atualizações do Microsoft 365 Apps com o Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  