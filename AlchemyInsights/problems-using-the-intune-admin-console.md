---
title: Problemas utilizando o console de administração do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944119"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemas utilizando o console de administração do Intune

**"Acesso negado" ao navegar pelo portal de administração do Intune.**

- Se você for um membro de uma função personalizada do Intune, certifique-se de que uma licença do Intune ou Enterprise Mobility Suite (EMS) está atribuída à sua conta.
- Se você estiver usando o Gerenciador de Configurações para gerenciar os dispositivos, certifique-se de que não faça parte da coleção de usuários do Intune para o Configuration Manager MDM.
- Verifique se você recebeu as permissões apropriadas do controle de administração baseado em função (RBAC) na lâmina funções do Intune.
- Verifique se o grupo usado não é uma lista de distribuição. O Intune no portal do Azure é compatível apenas com as contas de usuário que pertencem aos grupos de segurança do Azure Active Directory. Examine seus grupos no portal do Azure > **Intune** > **Grupos** ou no portal do Azure > **Azure Active Directory**.

**O usuário tem muitas permissões para a função atribuída do Intune**

Peça para o usuário acessar **Intune** > **funções do Intune** > **Minhas permissões** > **Exportar** para revisar as permissões concedidas.

**Adicionei um grupo de escopo a uma função, mas os usuários desse papel ainda poderão ver outros usuários ou dispositivos.**

Os grupos de escopo não filtram usuários ou dispositivos. Grupos de escopo:

- Limitar a quem os usuários podem atribuir políticas ou aplicativos.
- Permita que somente usuários específicos executem tarefas remotas em dispositivos.

Para obter mais informações sobre os grupos de escopo, confira [Controle de acesso baseado em função (RBAC) com o](https://docs.microsoft.com/intune/role-based-access-control)do Microsoft Intune.

**Adicionei um usuário a uma função do Intune, mas ainda temos acesso total ao console de administração do Intune.**

Navegue até o Intune > **Usuários** no portal do Azure e verifique se o usuário não está atribuído a nenhuma das funções a seguir no portal do Azure:

- Administrador global
- Administrador de Serviço do Intune
- Administrador do SharePoint

Confira [Controle de acesso baseado em função (RBAC) com o Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemas de Acesso**

Para saber mais, confira [Não é possível entrar no Office 365, no Azure ou no Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).