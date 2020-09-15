---
title: Abrir com o Explorer não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694444"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir com o Explorer não está funcionando

Se **Open com Explorer** ou **View no explorador de arquivos** não funcionar, certifique-se de que o serviço WebClient está definido para **executar** seguindo as etapas abaixo. Por exemplo, pode levar muito tempo para abrir uma biblioteca do SharePoint ou do OneDrive quando o serviço não estiver em execução. 
  
1. Na caixa Windows Search, digite Run, selecione o aplicativo da área de trabalho, digite Services. msc e selecione **Enter**.
    
2. Role para baixo até o serviço WebClient e verifique a coluna **status** . Se o status do serviço WebClient não estiver **em execução**, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique em **OK**. Habilite o serviço, se necessário, selecionando **manual** ou **automático** na caixa **tipo de inicialização** . 
    
> [!NOTE]
> Para solucionar problemas de abertura no explorador de arquivos, confira [abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explorar a sincronização como uma alternativa melhor: [sincronizar arquivos do SharePoint com o novo cliente de sincronização do onedrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

