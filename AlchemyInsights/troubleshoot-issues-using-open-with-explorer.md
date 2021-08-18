---
title: Solucionar problemas usando Abrir com o Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323554"
---
# <a name="fix-problems-with-open-with-explorer"></a>Corrigir problemas com o Open with Explorer

Correção de problemas comuns com a abertura de uma biblioteca de documentos SharePoint ou OneDrive usando o **comando Abrir com Explorer:** 
  
- Use Internet Explorer 10 ou Internet Explorer 11. **Abrir com o Explorer** não é compatível com Microsoft Edge, Google Chrome, Firefox e outros. **Abrir com o Explorer** está desabilitado em todos os navegadores, exceto no Internet Explorer. 
    
- **Abrir com o Explorer** não está disponível na experiência moderna para SharePoint bibliotecas. Use **View in File Explorer** em vez disso. Selecione **Exibir opções** Exibir no Explorador de \> **Arquivos**. O modo de exibição no Explorador de Arquivos não é compatível com Microsoft Edge, Google Chrome, Firefox e outros. **Exibir no Explorador de** Arquivos disponível somente no Internet Explorer. 
    
- Certifique-se de que o serviço WebClient está em execução. Na caixa Windows de pesquisa, digite executar, selecione o aplicativo da área de trabalho Executar, digite services.msc e pressione Enter. Role para baixo até o serviço WebClient e certifique-se de que a **coluna Status** exibe "Running". Se não, clique duas vezes no serviço, clique em **Iniciar** e clique em **OK**. (Talvez seja necessário habilitar primeiro o serviço selecionando **Manual** **ou Automático** na caixa Tipo **de** inicialização.) 
    
**Observação:** abrir uma biblioteca no Explorador de Arquivos é útil se você precisar copiar ou mover vários arquivos e pastas uma vez, mas se você quiser trabalhar regularmente na biblioteca, recomendamos sincroná-lo. Para solucionar problemas de abertura no Explorador de Arquivos, [consulte Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Para obter informações sobre como configurar a sincronização, consulte [Sync SharePoint files with the new Sincronização do OneDrive client](https://go.microsoft.com/fwlink/?linkid=871666).
  
Confira o artigo Como usar o comando "Abrir com [o Explorer"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) para solucionar problemas no SharePoint Online para obter mais informações. 
  

