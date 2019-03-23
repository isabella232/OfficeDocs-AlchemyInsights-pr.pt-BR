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
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764896"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir com o Explorer não está funcionando

Se **Open com Explorer** ou **View no explorador de arquivos** não funcionar, certifique-se de que o serviço WebClient está definido para **executar** seguindo as etapas abaixo. Por exemplo, pode levar muito tempo para abrir uma biblioteca do SharePoint ou do OneDrive quando o serviço não estiver em execução. 
  
1. Na caixa Windows Search, digite Run, selecione o aplicativo da área de trabalho, digite Services. msc e selecione **Enter**.
    
2. Role para baixo até o serviço webClient e verifique a coluna **status** . Se o status do serviço webClient não estiver **em execução**, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique em **OK**. Habilite o serviço, se necessário, selecionando **manual** ou **automático** na caixa **tipo de inicialização** . 
    
> [!NOTE]
> Para solucionar problemas de abertura no explorador de arquivos, confira [abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explorar a sincronização como uma alternativa melhor: [sincronizar arquivos do SharePoint com o novo cliente de sincronização do onedrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

