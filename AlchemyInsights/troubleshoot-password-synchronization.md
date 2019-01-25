---
title: Solucionar problemas de sincronização de senha
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457080"
---
# <a name="troubleshoot-password-synchronization"></a>Solucionar problemas de sincronização de senha

Para solucionar problemas em que nenhum senhas são sincronizados com a versão do Windows Azure Connect da AD 1.1.614.0 ou posterior:
  
1. Abra uma nova sessão do Windows PowerShell no seu servidor do Azure Connect do AD com a opção **Executar como administrador** . 
    
2. Execute **Set-ExecutionPolicy RemoteSigned** ou **Set-ExecutionPolicy irrestrito**. 
    
3. Inicie o Assistente de conectar do Azure AD.
    
4. Navegue até o * * tarefas adicionais * * página, selecione * * Troubleshoot * * e clique em **Avançar**. 
    
5. Na página de solução de problemas, clique em menu **Iniciar para iniciar a solução de problemas** no PowerShell. 
    
6. No menu principal, selecione **Solucionar problemas de sincronização de senha**. 
    
7. No menu sub, selecione a **sincronização de senha não funciona em todos os**. 
    
 **Compreender os resultados da tarefa a solução de problemas**
  
A tarefa de solução de problemas executa as seguintes verificações:
  
- Valida que o recurso de sincronização de senha está habilitado para seu locatário do Azure AD.
    
- Valida que o servidor Connect do Azure AD não está no modo de preparo.
    
- Para cada conector de Active Directory local existente, (que corresponde a uma floresta existente do Active Directory):
    
- 
  - Valida se o recurso de sincronização de senha está habilitado.
    
  - Procura eventos de pulsação de sincronização de senha nos logs de eventos do Windows.
    
  - Para cada domínio do Active Directory sob o conector do Active Directory local:
    
  - Valida que o domínio é acessível a partir do servidor Connect do Azure AD.
    
  - Valida que as contas de serviços de domínio Active Directory (AD DS) usadas pelo conector do Active Directory local tem o nome de usuário correto, senha e permissões necessárias para a sincronização de senha.
    
Para obter mais ajuda para solucionar problemas de sincronização de senha, consulte [Troubleshoot a sincronização de senha com a sincronização do Azure Connect do AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

