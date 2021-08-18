---
title: Problema ao ingressar em VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: d89fb92ce1775e5a77808a1893a315419b4d54706dc737327c51f7c4c4e488e2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088060"
---
# <a name="issue-joining-vms"></a>Problema ao ingressar em VMs

Para resolver problemas que ocorrem ao tentar ingressar em VMs, execute as etapas a seguir:

1. Tente entrar usando o formato **UPN** (por exemplo, 'joeuser@contoso.com') em vez do formato **SAMAccountName** ('CONTOSO\joeuser').
2. Certifique-se de ter habilitado a sincronização de senha de acordo com as etapas descritas no guia de *Introdução*.
3. Certifique-se de que a conta de usuário afetada não seja uma conta externa no locatário do Azure Active Directory. Os usuários externos não podem entrar no domínio gerenciado, pois os Azure AD Domain Services não têm credenciais para essas contas de usuário.
4. Se a conta de usuário afetada for uma conta de usuário somente na nuvem, verifique se os usuários alteraram suas senhas depois de habilitar os Azure AD Domain Services. Essa etapa faz com que os hashes de credencial obrigatório para os Azure AD Domain Services sejam gerados.
5. Se as contas de usuário afetadas forem sincronizadas de um diretório local, verifique se a versão recomendada do Azure AD Connect foi configurada para executar uma sincronização completa.
6. Se o problema persistir após a confirmação da Etapa 4, execute os seguintes comandos em seu computador de sincronização:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.