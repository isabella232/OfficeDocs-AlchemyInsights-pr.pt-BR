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
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321849"
---
# <a name="open-with-explorer-isnt-working"></a>Abrir com o Explorer não está funcionando

Se **Open with Explorer** ou View in File **Explorer** não funcionar, certifique-se de que o serviço WebClient está definido como Executando seguindo as etapas abaixo.  Por exemplo, pode levar muito tempo para abrir uma biblioteca SharePoint ou OneDrive quando o serviço não estiver em execução. 
  
1. Na caixa Windows de pesquisa, digite executar, selecione o aplicativo da área de trabalho Executar, digite services.msc e selecione **Enter**.
    
2. Role para baixo até o serviço WebClient e verifique a **coluna Status.** Se o status do serviço WebClient não estiver **Sendo Executado,** clique duas vezes no serviço, clique em Iniciar **e** clique em **OK**. Habilita o serviço, se necessário, selecionando **Manual** **ou Automático** na caixa **Tipo de** inicialização. 
    
**Observação:** para solucionar problemas de abertura no Explorador de Arquivos, [consulte Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore a sincronização como uma alternativa melhor: [sincronizar SharePoint arquivos com o novo Sincronização do OneDrive cliente](https://go.microsoft.com/fwlink/?linkid=871666). 
  

