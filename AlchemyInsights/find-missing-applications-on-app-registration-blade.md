---
title: Encontrar aplicativos ausentes na folha de registro de aplicativos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057090"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Encontrar aplicativos ausentes na folha de registro de aplicativos

1. Não é possível encontrar aplicativos no portal de Registro de Aplicativos.

    Se um aplicativo for um aplicativo de vários locatários e tiver sido registrado em outro locatário, ele não será exibido em Folha de Registro de Aplicativo. No entanto, você pode encontrá-lo em Enterprise de aplicativos depois que ela tiver sido acessada (depois de consentida) e a entidade de serviço tiver sido criada em seu locatário. Para obter mais informações, consulte [Aplicativos & entidades de serviço no Azure AD - plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Não é possível exibir aplicativos na folha Registro de Aplicativos, mesmo que você seja um administrador.

    Verifique se você está no diretório certo no portal do Azure.
3. Meu aplicativo não está listado na Enterprise Application, mas aparece quando eu consultava o comando do PowerShell.

    Às vezes, depois de excluir o aplicativo do portal do Azure, ele não aparece no portal, mas pode não ter sido excluído completamente. Para saber mais, confira:
    - Você pode recuperar a lista de aplicativos excluídos anteriormente e ver se o aplicativo aparece na lista usando o comando do Powershell: **Get-AzureADDeletedApplication**. Para saber mais, confira [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Se quiser remover completamente o aplicativo, você pode tentar o seguinte no PowerShell: **Remove-AzureADApplication -ObjectId**. Para saber mais, confira [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Como alternativa, você pode tentar restaurar o aplicativo excluído usando o seguinte comando do Powershell: **Restaurar AzureADDeletedApplication -ObjectId**. Para saber mais, confira [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Não é possível encontrar a lista de todos os aplicativos empresariais pré-instalados no meu novo locatário do Azure.

    Não há aplicativos empresariais pré-instalados no Azure AD por padrão. Você precisa adicioná-lo manualmente da opção "Novo aplicativo" navegando na galeria do Azure AD ou adicionando um aplicativo que não seja de galeria. Para saber mais, confira Início rápido: Adicionar um aplicativo ao [seu locatário Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Se você for um administrador global, poderá acessar facilmente seus aplicativos usando o [Microsoft 365 de aplicativos](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Não é possível encontrar meus aplicativos no portal Meus Aplicativos.

    Certifique-se de que os aplicativos não estão ocultos na página da coleção Meus Aplicativos. Para saber mais, confira [Coleções (visualização) no portal Meus Aplicativos - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Para iniciar aplicativos no portal Meus Aplicativos, consulte Localizar & aplicativos no portal Meus [Aplicativos - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 O aplicativo Mover não está sendo exibido na Enterprise Applications após a instalação.

    O aplicativo "Office 365 Mover" é um aplicativo multitenente que não precisa ser adicionado ao AAD usando a seção Aplicativos de Galeria em Registro Enterprise App. Para acessar Office 365 aplicativo Mover, basta entrar no aplicativo e solicitar o consentimento do usuário para as permissões. Depois que o usuário fornece o consentimento, esse aplicativo é adicionado automaticamente ao locatário com a id de email que você fez login.

    Depois de entrar no aplicativo, você poderá encontrar a entrada desse aplicativo sob a folha Enterprise Aplicativos no AAD. Você precisa pesquisar esse aplicativo digitando o nome completo, ou seja, "Office 365 Mover" ou simplesmente pesquisar "office" e ele deve listar o aplicativo. Para saber mais, consulte Office 365 Mover diz que ele já está instalado, mas não está listado na galeria Enterprise [Application.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. Início rápido: Exibir a lista de aplicativos que estão usando seu locatário do [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) para gerenciamento de identidade mostra como exibir os aplicativos, também conhecidos como aplicativos, que já estão definidos para usar seu locatário do Azure AD como seu Provedor de Identidade (IdP).
9. [Solucionar problemas comuns adicionando ou removendo](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) um aplicativo Azure Active Directory ajuda você a entender os problemas comuns que as pessoas enfrentam ao exibir aplicativos Azure Active Directory.
