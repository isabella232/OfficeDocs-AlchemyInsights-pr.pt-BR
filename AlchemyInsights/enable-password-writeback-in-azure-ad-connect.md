---
title: Habilitar o write-back de senha no Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118192"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Habilitar o write-back de senha no Azure AD Connect

Para habilitar o write-back da redefinição de senha por autoatendimento, habilite primeiro a opção de write-back no Azure AD Connect. A partir do seu servidor do Azure AD Connect, realize as seguintes etapas:

1. Entre no seu servidor Azure AD Connect e inicie o assistente de configuração do **Azure AD Connect**.
2. Na página **Bem-vindo**, clique em **Configurar**.
3. Na página **Tarefas adicionais**, clique em **Personalizar as opções de sincronização** e depois em **Avançar**.
4. Na página Conectar ao Azure AD, insira uma credencial de administrador global para o locatário do Azure e clique em Avançar.
5. Nas páginas **Conectar os diretórios** e **Filtrar domínio/UO**, clique em **Avançar**.
6. Na página **Recursos opcionais**, selecione a caixa ao lado de **Write-back de senha** e clique em **Avançar**.
7. Na página **Pronto para configurar**, clique em **Configurar** e aguarde que o processo seja concluído.
8. Ao concluir a configuração, clique em **Sair**.

Com o write-back de senha habilitado no Azure AD Connect, agora poderá configurar o SSPR do Azure AD para write-back.  Para habilitar o writeback de senha no SSPR, conclua as seguintes etapas:

1. Entre no portal do Azure usando uma conta de administrador global.
2. Pesquise e selecione o **Azure Active Directory**, clique em **Redefinição de senha** e escolha **Integração local**.
3. Definir a opção **Gravar as senhas em seu diretório local?** para **Sim**.
4. Defina a opção **Permitir que os usuários desbloqueiem contas sem redefinir a senha?** para **Sim**.
5. Quando estiver pronto, clique em **Salvar**.

Para saber mais, confira [Habilitar o write-back da redefinição de senha por autoatendimento do Azure Active Directory em um ambiente local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Quando um administrador redefine a senha de um usuário no portal do Microsoft Azure, se esse usuário for federado ou hash de senha sincronizada, a senha será gravada no local. Essa funcionalidade requer a Licença Premium do Azure (P1 ou P2) e atualmente não tem suporte no portal do Office Admin.
