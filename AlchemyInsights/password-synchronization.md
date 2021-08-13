---
title: Sincronização de senha
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960823"
---
# <a name="password-synchronization"></a>Sincronização de senha

**A Sincronização de Hash de Senha não funciona em nada**

Alguns problemas comuns que os clientes encontram quando a Sincronização de Hash de Senha não funciona são:

- A conta do Active Directory usada pelo Azure AD Conexão para se comunicar  com o  Active Directory local não é concedida Replicar Alterações de Diretório e Replicar Alterações de Diretório Todas as permissões, que são necessárias para sincronização de senhas - Você precisa corrigir isso concedendo essas permissões à conta do Active Directory.
- A sincronização de hash de senha é desabilitada  depois que um administrador alterou o método User Sign-In de Sincronização de Senha para outra opção, como Federação com **AD FS** no assistente do Azure AD Conexão - Você pode corrigir isso rehabilitando o recurso de sincronização de **hash** de senha no assistente de Conexão do Azure AD.
- Problema de conectividade com o Active Directory local. Por exemplo, alguns controladores de domínio não são acessíveis pelo [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Conexão, ou as portas necessárias são bloqueadas pelo Firewall - Você precisa corrigir isso garantindo que a conectividade entre o servidor do Azure AD Conexão e o Active Directory local funcione corretamente.
- O servidor do Azure AD Conexão está no modo de preparo, o que fará com que o servidor não consiga os hashes de senha - Para solucionar o problema, siga as etapas descritas na seção Solucionar problemas de sincronização de senha com a sincronização do [Azure AD Conexão -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Nenhuma senha é sincronizada .

**A Sincronização de Hash de Senha não funciona para alguns dos meus usuários**

1. Se você reparou que o hash de senha  não está sincronizando para um usuário, use a tarefa de solução de problemas no Azure AD Conexão investigar e resolver o problema. Execute as seguintes tarefas:

    a. [Executar a tarefa de solução de problemas no assistente](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Use o cmdlet de solução de problemas para investigar o problema de sincronização de hash de senha para um uso específico](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. O objeto Usuário do Active Directory local está habilitado para que o Usuário altere a **senha na próxima opção de logon.** Quando essa opção estiver habilitada, o usuário receberá uma senha temporária e será solicitado a alterar a senha no próximo logon. O Azure AD Conexão não sincroniza senhas temporárias com o Azure AD.

Para resolver o problema acima, execute uma das seguintes tarefas:

- Peça ao usuário para entrar no aplicativo local (por exemplo, Windows Desktop) e alterar a senha. A nova senha será sincronizada com o Azure AD.
- Fazer com que um administrador atualize a senha do usuário sem habilbilcar a opção O usuário deve alterar a senha no próximo **logon** e compartilhar a nova senha com o usuário.

3. O objeto Usuário do Active Directory local não **está configurado corretamente** para sincronização de objetos ou sincronização de senha. Para solucionar esse problema, siga as etapas descritas na sincronização de hash de senha de solução de problemas com o [Azure AD Conexão sincronização](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







