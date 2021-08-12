---
title: Solucionar problemas de grupo
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
- "7814"
- "9004358"
ms.openlocfilehash: 47f00118a5a4b446b6a3b06f0fc6101d00d11b626eaf249bb6ca962a55f7f4d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939331"
---
# <a name="troubleshoot-group-issues"></a>Solucionar problemas de grupo

**Preciso atribuir um grupo a uma função do Azure AD**

Para atribuir um grupo do Azure Active Directory (AD) a uma função do Azure AD, execute as seguintes etapas:

1. Crie um novo grupo - Para criar um novo grupo:

    a. Entre no centro de administração do Azure AD com permissões de administrador global ou de administrador de funções com privilégios. 
    b. Selecione Azure Active Directory > Grupos > Todos os grupos > Novo grupo. 
    c. Crie o grupo.

2. Atribua a função ao grupo durante a criação do grupo ou após a criação do grupo.

    a. Para atribuir uma função ao grupo no momento da sua criação, altere as funções do Microsoft Azure AD que podem ser atribuídas ao grupo e crie o grupo.
    b. Para atribuir uma função ao grupo após sua criação, navegue até a guia Funções atribuídas para o grupo recém-criado e atribua a função ao grupo.

**Preciso gerenciar a associação de um grupo atribuído à função do Azure AD**

1. Para evitar a elevação de privilégios, por padrão, somente o administrador de funções com privilégios e o administrador global podem modificar a associação de um grupo atribuído a uma função. No entanto, eles podem optar por atribuir um proprietário a esse grupo e delegar essa tarefa. Para saber mais, confira [Usar grupos de nuvem para gerenciar atribuições de função no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Para perguntas comuns e dicas de solução de problemas para atribuição de funções a grupos no Azure AD, confira [Solução de problemas de funções atribuídas a grupos de nuvem](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Grupos dinâmicos**

1. Se você não conseguir encontrar os atributos de usuário integrados, verifique se o atributo está na lista de propriedades com suporte.
2. Se você estiver procurando atributos de dispositivo integrados, verifique se o atributo está na lista de atributos do dispositivo 
3. Além dos atributos de usuário e de dispositivo integrados, você também pode usar [Atributos de Extensão](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Após sincronizar os atributos de extensão do AD do Windows Server local ou de uma aplicativo SaaS conectado, os atributos devem estar visíveis na lista suspensa do construtor de regras. O nome do atributo personalizado pode ser encontrado no diretório ao consultar o atributo de um usuário usando o PowerShell e pesquisando o nome do atributo. Eles também podem ser usados ao construir regras na sintaxe da regra.
4. Verifique se o locatário tem a licença apropriada. Os grupos dinâmicos exigem que o locatário tenha uma licença do Azure AD P1 Premium. Acesse a lista de planos de licença do Azure AD [aqui](https://azure.microsoft.com/pricing/details/active-directory/). Acesse os planos de licenciamento do Enterprise Mobility + Security [aqui](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Verifique se a função do usuário que cria o grupo dinâmico é administrador global, administrador do intune, administrador de grupo ou administrador de usuário.
6. Aguarde até o grupo ser preenchido. Dependendo do tamanho do locatário, o grupo poderá demorar até 24 horas para ser preenchido pela primeira vez ou após uma alteração de regra.
7. Para saber mais, confira [Criar regras baseadas em atributo para associação de grupo dinâmica](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Preciso excluir um grupo**

1. Os grupos podem ser excluídos do diretório usando o cmdlet Remove-AzureADGroup no módulo do PowerShell do Azure AD.
2. Antes de tentar excluir um grupo sincronizado no Azure AD, verifique se você excluiu todas as licenças atribuídas para evitar erros.
3. Para saber mais sobre como excluir grupos, confira [Excluir um grupo com uma licença atribuída](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Preciso restaurar um grupo excluído**

1. Se um grupo do Office 365 for excluído, ele só poderá ser restaurado até 30 dias antes da exclusão permanente. Após a exclusão permanente, o grupo não poderá mais ser restaurado. Saiba mais sobre a restauração de grupos [aqui](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Não há suporte para esta funcionalidade para grupos de segurança e grupos de distribuição.
3. Verifique se você tem autorização para restaurar um grupo do Office 365. Administradores globais, administradores de grupo, administradores de contas de usuário, administradores de serviços do Intune, suporte de camada1 de parceiro ou camada2, e o proprietário do grupo podem restaurar um grupo.
4. Quando um grupo dinâmico é excluído e restaurado, ele é visto como um novo grupo e preenchido novamente de acordo com a regra. Esse processo pode demorar 24 horas.
5. Para saber mais sobre como restaurar um grupo excluído, confira [Restaurar um grupo do Office 365 excluído no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Configuração da política de expiração de grupo**

1. Só há suporte para essa funcionalidade para grupos do Office 365, e não para grupos de segurança e grupos de distribuição.
2. Configurar e usar a política de expiração para grupos do Office 365 requer uma licença do Azure AD Premium.
3. Atualmente, só é possível configurar uma política de expiração para grupos do Office 365 em um locatário.
4. Somente administradores globais, administradores de grupo, administradores de usuários e o proprietário do grupo podem renovar um grupo.
5. Se um grupo do Office 365 expirar, ele será excluído e só poderá ser restaurado até 30 dias antes da exclusão permanente. Após a exclusão permanente, o grupo não poderá mais ser restaurado. Saiba mais sobre a restauração de grupos [aqui](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Renovação automática com base na atividade**

As atividades dos usuários do SharePoint, do Outlook e do Teams podem acionar a renovação automática do grupo. As atividades são verificadas com 35 dias antes da expiração de um grupo. Se houver atividade durante o atual ciclo de vida do grupo, o grupo será automaticamente renovado e a notificação por email não será enviada aos proprietários do grupo.

**Tempo de notificação para grupos expirados**

1. As notificações por email são enviadas aos proprietários do grupo do Office 365 com 30 dias, 15 dias e 1 dia antes da expiração do grupo.
2. Ao configurar a expiração pela primeira vez, qualquer grupo que for mais antigo que o intervalo de expiração será definido para 35 dias até a expiração.
3. A data de expiração do grupo é calculada com base na data de renovação do grupo, não com base na data de atualização da política. Se a política de expiração for atualizada, a data de vencimento não será alterada.
4. Para saber mais, confira [Política de Expiração de Grupo e emails de renovação](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) e [Restaurar um grupo do Office 365 excluído no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Permissão para criar um grupo**

Verifique se você tem autorização para criar um novo usuário padrão. Os administradores globais podem desabilitar a criação de grupos no portal do Azure ou no Painel de Acesso. Talvez você precise de um administrador para criar o novo grupo para você ou para lhe dar as permissões apropriadas.

1. [Criar um novo grupo e adicionar membros no portal do Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Criar grupos no MSOnline do Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Desabilitar a criação de grupos no Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Gerenciar quem pode criar grupos do Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Desabilitar a notificação de boas-vindas do Office 365 via Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Funções administrativas do Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Gerenciar permissões de criação de grupo**

1. Os administradores globais podem gerenciar as permissões de criação de grupo para segurança ou grupos Office 365 criados no portal Azure ou no Painel de Acesso, definindo que os **Usuários podem criar grupos de segurança nos portais Azure** ou que os **Usuários podem criar grupos do Office 365 nas configurações dos portais do Azure** em **Todos os grupos > Geral (Configurações)**.
2. Você também pode restringir a criação de grupos para selecionar um grupo de usuários se você tiver uma licença do Azure AD P1 Premium.

**Desabilitar a notificação de boas-vindas para novos membros de um grupo do Office 365**

A notificação de boas-vindas enviada aos usuários que são adicionados aos grupos do Office 365 pode ser desabilitada definindo `UnifiedGroupWelcomeMessageEnabled` como **False** no Powershell. Saiba mais sobre essa configuração [aqui](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













