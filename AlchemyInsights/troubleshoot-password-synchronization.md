---
title: Solucionar problemas de sincronização de senha
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664914"
---
# <a name="troubleshoot-password-synchronization"></a>Solucionar problemas de sincronização de senha

Para solucionar problemas de sincronização de senha, comece usando esta tarefa de solução de problemas do AAD Connect para determinar por que as senhas não estão sendo sincronizadas. Para começar, vá para [gerenciar a sincronização direta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Abra uma nova sessão do Windows PowerShell em seu servidor do Azure AD Connect e selecione a opção **Executar como administrador** .

2. Execute Set-ExecutionPolicy RemoteSigned ou Set-ExecutionPolicy Unrestricted.

3. Inicie o assistente do Azure AD Connect.

4. Vá até a página tarefas adicionais > **solucionar problemas**  >  **em seguida**.

5. Selecione **Iniciar** para abrir o menu de solução de problemas do PowerShell.

6. Selecione **solucionar problemas de sincronização de senha**.

    Normalmente, o problema é que uma senha não é sincronizada para uma conta de usuário específica.

    **Anotações** A sincronização de senha falha se a última sincronização de senha bem-sucedida ocorreu algum tempo atrás.

Para obter mais ajuda para a solução de problemas de sincronização de senha, consulte [Troubleshoot password hash Synchronization with Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).