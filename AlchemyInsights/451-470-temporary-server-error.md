---
title: 451 4.7.0 Erro de servidor temporário. Tente novamente mais tarde. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: 16e16f087c2b13a9ad5fec7223b4f3395e42646e
ms.sourcegitcommit: 380ee556007d2be389b1a99795bca04bc1f9f60f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2021
ms.locfileid: "53604910"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Erro de servidor temporário. Tente novamente mais tarde. PRX4

Você pode enfrentar um problema ao enviar emails por meio do Smarthost "smtp.office365.com" usando o método de Envio de Cliente SMTP e receber o erro: "Erro de servidor temporário 451 4.7.0. Tente novamente mais tarde. PRX4 é principalmente temporário." 

Certifique-se de que você não está usando uma caixa de correio compartilhada para Envio de Cliente SMTP, pois o método de Envio de cliente SMTP requer uma caixa de correio licenciada para enviar emails. No entanto, se você não estiver usando uma caixa de correio compartilhada e o problema persistir, verifique o seguinte:

1. Habilitar o envio SMTP do Cliente na caixa de correio licenciada que está sendo usada executando este comando do PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OU

    1. Vá para o Centro de administração do Microsoft 365 > **usuários ativos** e selecione o usuário.
    1. Vá para a guia Email > **Aplicativos de email >** selecione **Gerenciar aplicativos de email**. 
    1. Certifique-se **de que a configuração SMTP** autenticada está marcada (habilitada).
    1. Selecionar **Salvar alterações**.
    
    Para habilitar a Autenticação SMTP para uma organização inteira, execute este comando:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Observação**: por motivos de segurança, é recomendável habilitar a Autenticação SMTP somente para a caixa de correio que está sendo usada. A configuração de nível do usuário substitui a configuração de nível da organização.

2. Desabilitar os padrões de segurança do Azure ao ativar **padrões de segurança** como **Não**:

    1. Entre no portal do Azure como administrador de segurança, administrador de Acesso Condicional ou administrador global.
    1. Navegue até Azure Active Directory >**  Propriedades** e selecione **Gerenciar padrões de segurança.**
    1. Definir a **alternância Habilitar padrões** de segurança como **Não**.
    1. Selecione **Salvar**.

3. Desabilite a Autenticação Multifafatória (MFA) na caixa de correio licenciada que está sendo usada.

    1. Vá para o Centro de administração do Microsoft 365 e, no menu de navegação à esquerda, escolha **Usuários**  >  **Usuários ativos**.
    1. Na página **Usuários ativos**, escolha **Autenticação multifator**.
    1. Selecione o usuário e desabilite **a autenticação multifator**.

