---
title: Habilitar autenticação SMTP e solução de problemas
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
- "3000003"
- "5652"
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957196"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Habilitar autenticação SMTP e solução de problemas

Se quiser habilitar a autenticação SMTP para uma caixa de correio ou estiver recebendo um erro "Cliente não autenticado", "Autenticação malsucedida" ou "SmtpClientAuthentication" com o código 5.7.57 ou 5.7.3 ou 5.7.139 ao tentar retransmitir emails autenticando um dispositivo ou aplicativo com o Microsoft 365, execute estas três ações para resolver o problema:

1. Desabilite o [padrão de segurança do Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) alternando **Habilitar padrões de segurança** para **Não**.

    Entre no portal do Azure como administrador de segurança, administrador de acesso condicional ou administrador global.<BR/>
    b. Navegue até Azure Active Directory > **Propriedades**.<BR/>
    c. Selecione **Gerenciar padrões de segurança**.<BR/>
    d. Defina **Habilitar padrões de segurança** para **Não**.<BR/>
    e. Selecione **Salvar**.

2. [Habilite o envio de cliente SMTP](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) na caixa de correio licenciada.

    a. No Centro de administração do Microsoft 365, acesse **Usuários ativos** e selecione o usuário.<BR/>
    b. Vá para a guia Email e, em **Aplicativos de email**, selecione **Gerenciar aplicativos de email**.<BR/>
    d. Verifique se o **SMTP autenticado** está marcado (habilitado).<BR/>
    e. Selecione **Salvar alterações**.<BR/>

3. [Desabilite a autenticação multifator (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) na caixa de correio licenciada.

    a. Vá para o Centro de administração do Microsoft 365 e, no menu de navegação à esquerda, selecione **Usuários** > **Usuários ativos**.<BR/>
    b. Selecione **Autenticação multifator**.<BR/>
    c. Selecione o usuário e desabilite a **Autenticação multifator**.<BR/>
