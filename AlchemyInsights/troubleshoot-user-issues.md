---
title: Solucionar problemas do usuário
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886770"
---
# <a name="announcements"></a>Comunicados

Siga as orientações do Google sobre teste de compatibilidade para testar se seus aplicativos são afetados. As orientações do Google estão disponíveis em https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support.

Certifique-se de usar o modo de exibição da Web do sistema ou o navegador do sistema ao conectar seus usuários com contas pessoais do Google. Para obter mais informações, confira [Problemas para entrar nos aplicativos usando apenas o navegador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Não consigo criar um novo usuário no meu Azure Active Directory**

Para solucionar o problema de não poder criar um novo usuário no Azure AD, execute as seguintes etapas:

1. Certifique-se de que você está autorizado a criar um novo usuário padrão. Somente a função de administrador global ou administrador de usuário no Azure Active Directory (AD) pode criar um novo usuário padrão. Se você não estiver em uma dessas funções, peça a um administrador para adicioná-lo a uma dessas funções ou para criar uma nova conta de usuário para você.
2. Certifique-se de que o nome de usuário esteja em um domínio verificado no Azure AD. Se você não tiver nenhum nome de domínio personalizado verificado no seu Azure AD, poderá usar o domínio inicial do Azure AD, que termina com *.onmicrosoft.com.
3. Certifique-se de que o nome de usuário esteja em um domínio não federado ao Azure AD do seu AD local. Os usuários não podem ser adicionados à nuvem com nomes de domínio federados no local.
4. Certifique-se de que nenhum outro usuário ou contato já tenha o nome de usuário que você deseja atribuir ao novo usuário. Os nomes de usuário devem ser exclusivos no Azure AD.
5. Confira as [Funções e administradores do Azure AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para o seu Azure AD.
6. Confira os [nomes de domínio](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) para o seu Azure AD.
7. Revise os [logs de auditoria](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) para ver informações mais detalhadas sobre um usuário criado ou excluído recentemente, como quem executou a ação e quando.
8. Para saber mais sobre como adicionar novos usuários, confira [Usar o portal do Azure para criar um novo usuário no Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory).
9. Para saber mais sobre as permissões de função de administrador do Azure AD, confira [Funções administrativas do Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Para obter detalhes sobre como criar um usuário usando o Powershell do Azure AD, confira [PowerShell do Azure AD para criar um novo](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problema com a inscrição de autoatendimento**

Para solucionar problemas relacionados à inscrição de autoatendimento, execute as seguintes etapas:

1. Para usar a inscrição de autoatendimento em seus aplicativos, primeiro habilite a inscrição de autoatendimento do locatário. 
2. Para habilitar um aplicativo para oferecer suporte à inscrição de autoatendimento, adicione-o ao fluxo do usuário. Na próxima vez que acessar a página de logon desse aplicativo, você verá uma opção **_Não tem uma conta? Crie uma!_* _. Isso inicia o processo de inscrição de autoatendimento.
3. Para obter informações sobre como usar a inscrição de autoatendimento para preencher uma organização no Azure AD, confira [Inscrição de autoatendimento no Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Depois de associar o fluxo do usuário a um ou mais aplicativos, os usuários que visitam esse aplicativo poderão se inscrever e obter uma conta de convidado usando as opções configuradas no fluxo do usuário. Para obter mais informações sobre como se inscrever e obter uma conta de convidado, os usuários podem conferir [Inscrição de autoatendimento para usuários convidados](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problema ao convidar um usuário externo**

Para solucionar problemas relacionados ao convite de um usuário externo, execute a seguinte etapa:

Certifique-se de enviar o convite do usuário ao endereço de email que corresponda ao nome com o qual o usuário faz logon. Se você enviar o convite para o endereço de email proxy de um usuário, ele não poderá resgatá-lo. Para obter mais informações, confira [documentação B2B do Azure AD](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Não consigo atribuir licenças a um usuário**

Para solucionar problemas relacionados à atribuição de licenças a um usuário, execute as seguintes etapas:

1. Para gerenciar licenças de usuário, certifique-se de usar uma conta com uma das funções de administrador necessárias: administrador global, administrador de licença ou administrador de usuário. Você pode verificar a função do usuário na guia **Função do diretório** na folha do usuário.
2. Se você estiver usando o portal do Azure e a atribuição de licença falhar, clique na notificação no canto superior direito. Isso abre uma folha com detalhes sobre o que deu errado. Na maioria dos casos, isso é suficiente para compreender e resolver o problema.
3. Antes que uma licença possa ser atribuída a um usuário, certifique-se de que a propriedade **Local de uso** esteja definida para o usuário. Verifique se o usuário tem essa propriedade definida, exibindo a guia **Perfil** na folha do usuário.
4. Certifique-se de que haja licenças disponíveis suficientes para o produto que você está tentando atribuir. Você pode ver o número de licenças disponíveis no portal do Azure, em [Azure Active Directory -> Licenças -> Todos os produtos](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. O usuário pode já ter outra licença cujos serviços estão em conflito com os da nova licença que você está tentando atribuir. Por exemplo, se o usuário tiver o serviço Exchange Online (Plano 1) habilitado, você não poderá atribuir uma licença com o Exchange Online (Plano 2). Desabilite um dos serviços para permitir a atribuição da nova licença. Se estiver usando o portal do Azure ou cmdlets do PowerShell, a página de **detalhes do problema** lista os serviços específicos que estão causando o conflito.
6. Se estiver tentando remover uma licença e não conseguir, o usuário pode ter outras licenças com serviços que dependem dos serviços que você está tentando remover. Se estiver usando o portal do Azure ou cmdlets do PowerShell, a mensagem de erro listará os serviços específicos que possuem dependências.
7. Se quiser entender por que uma licença foi adicionada/removida de um usuário (por exemplo, quem mais em sua organização pode ter feito alterações), verifique os logs de auditoria. Defina o filtro para **licenciar atividades** para mostrar todas as modificações, incluindo o "ator" que as executou.
8. Se estiver usando o Exchange Online, alguns usuários em seu locatário podem estar configurados incorretamente com o mesmo valor de endereço proxy. Nesses casos, você poderá ver mensagens de erro genéricas quando uma operação de licença falhar. [Este artigo](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contém mais informações sobre esse problema, incluindo informações sobre [como se conectar ao Exchange Online usando o PowerShell remoto](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Para identificar quais usuários em seu locatário contêm o mesmo endereço proxy, execute este cmdlet do Exchange Online:

Executar

Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses





