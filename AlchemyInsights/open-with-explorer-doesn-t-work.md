---
title: Abrir com o Explorer não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538448"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir com o Explorer não está funcionando

Se **Open com Explorer** ou **View no explorador de arquivos** não funcionar, certifique-se de que o serviço WebClient está definido para **executar** seguindo as etapas abaixo. Por exemplo, pode levar muito tempo para abrir uma biblioteca do SharePoint ou do OneDrive quando o serviço não estiver em execução. 
  
1. Na caixa Windows Search, digite Run, selecione o aplicativo da área de trabalho, digite Services. msc e selecione **Enter**.
    
2. Role para baixo até o serviço WebClient e verifique a coluna **status** . Se o status do serviço WebClient não estiver **em execução**, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique em **OK**. Habilite o serviço, se necessário, selecionando **manual** ou **automático** na caixa **tipo de inicialização** . 
    
> [!NOTE]
> Para solucionar problemas de abertura no explorador de arquivos, confira [abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explorar a sincronização como uma alternativa melhor: [sincronizar arquivos do SharePoint com o novo cliente de sincronização do onedrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

