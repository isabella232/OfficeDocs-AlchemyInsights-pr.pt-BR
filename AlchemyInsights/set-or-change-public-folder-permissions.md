---
title: Definir ou alterar permissões de pasta pública
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1868b8b04df012d44781f86ee75120ca443af5be5801074329f17c0e40a5acc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060880"
---
# <a name="permissions-and-public-folders"></a>Permissões e Pastas Públicas

Você pode alterar as permissões em suas Pastas Públicas usando Outlook, o centro de administração Exchange (EAC) ou o PowerShell:
  
- Para Outlook instruções, [clique aqui](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).
    
- Para o EAC, consulte [este artigo para](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) obter instruções. 
    
- Para o Powershell, consulte [este artigo para](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) obter instruções sobre como usar o Add-PublicFolderClientPermission commandlet. Se você precisar de instruções para se conectar ao Exchange Powershell, clique [aqui](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).
    
Se **os usuários externos** não puderem enviar emails para uma Pasta Pública habilitada para email, o motivo pode ser que a pasta pública está sem permissões necessárias para a entrega de emails externos. Você pode corrigir isso usando as instruções Outlook [aqui](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), ou as instruções do PowerShell [aqui](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).
  

