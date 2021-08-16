---
title: Não é possível acessar o Centro de administração do SharePoint ou do OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020432"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Não é possível acessar o Centro de administração do SharePoint ou do OneDrive

- Se o seu site do Centro de administração do SharePoint ou do OneDrive estiver inacessível ou não estiver disponível, poderá haver um problema de serviço temporário em que os usuários têm atrasos intermitentes ou erros de navegação ao acessar sites do SharePoint ou conteúdo do OneDrive. Marque o [Painel de integridade do serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se sua organização é afetada.

- É necessário atribuir uma licença do SharePoint aos administradores globais e do SharePoint. As contas recém criadas atribuídas à uma licença do SharePoint ou Função de administrador podem ter problemas para acessar o SharePoint, como "acesso negado" ou "o usuário não encontrado". Aguarde pelo menos 24 horas para que a sincronização seja concluída em nossos sistemas. Entendemos que 24 horas podem parecer muito tempo. Em muitos casos, já estamos trabalhando em uma solução.

- Os usuários do Gerenciamento de Identidades Privilegiado ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) poderão ter o acesso negado se a janela de tempo de acesso for muito pequena. Confira [Acesso negado a contas PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).