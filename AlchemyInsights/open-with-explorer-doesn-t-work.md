---
title: Abrir com Explorer não funciona
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456597"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir com Explorer não está funcionando

Se **Abrir com Explorer** ou **modo de exibição no Gerenciador de arquivos** não funcionar, verifique se que o serviço de cliente está definido para **execução** seguindo as etapas abaixo. Por exemplo, ela pode levar muito tempo para abrir uma biblioteca do SharePoint ou OneDrive quando o serviço não está sendo executado. 
  
1. Na caixa de pesquisa do Windows, digite executar, selecione o aplicativo da área de trabalho, Services. msc do tipo e selecione **Enter**a executar.
    
2. Role para baixo até o serviço de cliente e verifique a coluna **Status** . Se o status do serviço de cliente não estiver **em execução**, clique duas vezes em serviço, clique em **Iniciar**e, em seguida, clique em **Okey**. Habilite o serviço, se necessário, selecionando **Manual** ou **automático** na caixa **tipo de inicialização** . 
    
> [!NOTE]
> Para solucionar problemas de abertura no Gerenciador de arquivos, consulte [Abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore a sincronização como uma alternativa melhor: [arquivos de sincronização do SharePoint com o novo cliente de sincronização do OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

