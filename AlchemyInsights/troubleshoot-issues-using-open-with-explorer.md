---
title: Solucionar problemas usando abrir com o Explorer
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659046"
---
# <a name="fix-problems-with-open-with-explorer"></a>Corrigir problemas com abrir com o Explorer

Correção de problemas comuns com a abertura de uma biblioteca de documentos no SharePoint ou no OneDrive usando o comando **abrir com Explorer** : 
  
- Use o Internet Explorer 10 ou o Internet Explorer 11. **Abrir com o Explorer** não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros. **Abrir com o Explorer** está desabilitado em todos os navegadores, exceto no Internet Explorer. 
    
- **Abrir com o Explorer** não está disponível na experiência moderna para bibliotecas do SharePoint. Em vez disso, use o **modo de exibição no explorador de arquivos** . Selecione **Exibir opções** \> **Exibir no explorador de arquivos**. O modo de exibição no explorador de arquivos não é compatível com o Microsoft Edge, Google Chrome, Firefox e outros. **Exibir no explorador de arquivos** somente disponível no Internet Explorer. 
    
- Verifique se o serviço WebClient está em execução. Na caixa Windows Search, digite Run, selecione o aplicativo da área de trabalho, digite Services. msc e pressione Enter. Role para baixo até o serviço WebClient e verifique se a coluna **status** exibe "em execução". Caso contrário, clique duas vezes no serviço, clique em **Iniciar**e, em seguida, clique em **OK**. (Talvez seja necessário primeiro habilitar o serviço selecionando **manual** ou **automático** na caixa tipo de **inicialização** .) 
    
> [!NOTE]
> A abertura de uma biblioteca no explorador de arquivos é útil se você precisar copiar ou mover vários arquivos e pastas uma vez, mas se quiser trabalhar regularmente na biblioteca, recomendamos sincronizá-lo. Para solucionar problemas de abertura no explorador de arquivos, confira [abrir no Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Para obter informações sobre como configurar a sincronização, consulte [sincronizar arquivos do SharePoint com o novo cliente de sincronização do onedrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Confira o artigo [como usar o comando "abrir com o Explorer" para solucionar problemas no SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) para obter mais informações. 
  

