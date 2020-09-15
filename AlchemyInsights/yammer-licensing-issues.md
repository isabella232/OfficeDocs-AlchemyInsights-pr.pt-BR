---
title: Problemas de licenciamento do Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657264"
---
# <a name="yammer-licensing-issues"></a>Problemas de licenciamento do Yammer

Todos os usuários devem ter uma licença para usar o serviço do Yammer Enterprise, mas, por padrão, o Yammer não requer que os usuários tenham uma licença para acessar o serviço. Quando um administrador muda as configurações para bloquear usuários do Microsoft 365 sem as licenças do Yammer, usuários que não tem uma licença Yammer Enterprise não podem acessar o serviço. Para saber mais, confira [Gerenciar licenças de usuário do Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Quando as licenças são removidas dos usuários, o bloco do Yammer não é mais exibido, e outros serviços podem usar a remoção da licença para ocultar recursos. Em outros casos, os recursos ainda podem ser exibidos mas exigem uma licença para operar.  

**A licença não está sendo atualizada para o usuário**  

Ocasionalmente, o usuário é dado uma licença mas ainda não consegue acessar o Yammer. Os atrasos têm maior probabilidade de ocorrer quando uma atribuição de licença em massa está em andamento. Os usuários do Yammer não podem ser atualizados na mesma ordem em que as licenças são modificadas no Azure AD porque o sistema é executado de forma assíncrona. Aguarde até 24 horas antes de abrir um caso de suporte para informar problemas de sincronização de licença.  

**Atribuição de licenças em massa**  

Licenças podem ser atribuídas pelo centro de administração ou script do PowerShell. Para saber mais, confira [Atribuir licenças à usuários](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)e[Atribuir licenças para contas de usuários com Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

O suporte da Microsoft não fornece assistência criando scripts mas documentação de atribuição de licenças no Yammer está disponível. Para saber mais, confira [Gerenciar licenças do Yammer usando Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).