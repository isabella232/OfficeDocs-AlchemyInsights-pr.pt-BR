---
title: Solucionar problemas de sincronização de senhas
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
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105736"
---
# <a name="troubleshoot-password-synchronization"></a>Solucionar problemas de sincronização de senhas

Para solucionar problemas de sincronização de senhas, comece usando essa tarefa Conexão solução de problemas do AAD para determinar por que as senhas não estão sincronizadas. Para começar, vá para [Gerenciar sincronização direta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Abra uma nova sessão Windows PowerShell no servidor do Azure AD Conexão e selecione a opção **Executar como** Administrador.

2. Execute Set-ExecutionPolicy RemoteSigned ou Set-ExecutionPolicy Irrestrita.

3. Inicie o assistente de Conexão Azure AD.

4. Vá para a página Tarefas Adicionais > **Solução de** Problemas  >  **Em Seguida**.

5. Selecione **Iniciar** para abrir o menu solução de problemas do PowerShell.

6. Selecione **Solucionar Problemas de Sincronização de Senhas**.

    O problema geralmente é que uma senha não é sincronizada para uma conta de usuário específica.

    **Observações** A sincronização de senha falhará se a última sincronização de senha bem-sucedida foi há algum tempo.

Para obter mais ajuda para solucionar problemas de sincronização de senha, consulte Solucionar problemas de sincronização de hash de senha com o [Azure AD Conexão sincronização](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).