---
title: Solucionar problemas de sincronização de senha
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533795"
---
# <a name="troubleshoot-password-synchronization"></a>Solucionar problemas de sincronização de senha

Para solucionar problemas em que nenhuma senha é sincronizada com o Azure AD Connect versão 1.1.614.0 ou posterior:
  
1. Abra uma nova sessão do Windows PowerShell em seu servidor do Azure AD Connect com a opção **Executar como administrador** .

2. Execute **Set-ExecutionPolicy RemoteSigned** ou **Set-ExecutionPolicy Unrestricted**.

3. Inicie o assistente do Azure AD Connect.

4. Navegue até a página **tarefas adicionais** , selecione **solução de problemas**e clique em **Avançar**.

5. Na página solução de problemas, clique em **Iniciar para iniciar o menu solução de problemas** no PowerShell.

6. No menu principal, selecione **solucionar problemas de sincronização de senha**.

7. No menu sub, selecione a **sincronização de senha não funciona de**forma alguma.

**Entender os resultados da tarefa de solução de problemas**
  
A tarefa de solução de problemas executa as seguintes verificações:
  
- Valida que o recurso de sincronização de senha está habilitado para o locatário do Azure AD.

- Valida se o servidor do Azure AD Connect não está no modo de preparação.

- Para cada conector local existente do Active Directory (que corresponde a uma floresta existente do Active Directory):

- 
  - Valida se o recurso de sincronização de senha está habilitado.

  - Procura eventos de pulsação de sincronização de senha nos logs de eventos de aplicativos do Windows.

  - Para cada domínio do Active Directory sob o conector local do Active Directory:

  - Valida se o domínio pode ser acessado pelo servidor do Azure AD Connect.

  - Valida que as contas dos serviços de domínio Active Directory (AD DS) usadas pelo conector do Active Directory local tem o nome de usuário, senha e permissões corretos necessários para a sincronização de senha.

Para saber mais sobre como solucionar problemas de sincronização de senha, confira [solucionar problemas de sincronização de senha com o Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)
  