---
title: Solucionar problemas de SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428506"
---
# <a name="troubleshoot-sspr"></a>Solucionar problemas de SSPR

**Estou com problemas para configurar a redefinição de senha**

- Se você for administrador e estiver procurando como habilitar a redefinição de senha de autoatendados, consulte [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization. Você também pode querer revisar os [requisitos de licenciamento.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Você deve ter pelo menos uma licença atribuída em sua organização.
    - **Usuários somente na nuvem** - Qualquer SKU pago do Office 365 (O365) ou do Azure AD Basic
    - Usuários na nuvem **e/ou** locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
- Para obter perguntas adicionais sobre a redefinição de senha de autoatendados, revise [nossas perguntas frequentes.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Estou recebendo uma mensagem de erro**

Revise este artigo para encontrar erros comuns e suas soluções: Solucionar problemas de redefinição de senha [de autoatendificação](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Estou tendo um problema com minha política de redefinição de senha**

- Se sua política de redefinição de senha não estiver se comportando como esperado ou se você tiver dúvidas sobre políticas de redefinição de senha, revise este artigo: Políticas e restrições de senha no [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- As políticas de redefinição de senha não se aplicam aos administradores. A Microsoft impõe uma política de redefinição de senha de dois portais padrão forte para qualquer função de administrador do Azure. Certifique-se de que você está testando com um usuário que não seja um administrador. Para obter mais informações sobre a política de redefinição do administrador, consulte este artigo: [Diferenças de política de redefinição de administrador.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Não quero que meus usuários registrem informações de segurança adicionais para redefinição de senha**

Você pode preencher previamente dados (atributos de email e telefone) para seus usuários usando uma API, o PowerShell ou o Azure AD Connect. Para saber como ler:

- [Implantando redefinição de senha sem exigir que os usuários se registrem](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Quais dados são usados pela redefinição de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Quero que meus usuários registrem suas informações de segurança adicionais para redefinição de senha**

1. Faça com que seus usuários registrem suas informações de segurança para redefinição de senha de autoatendados direcionando-os [para](https://mysignins.microsoft.com/security-info)aka.ms/ssprsetup .
1. Depois que os dados são preenchidos para o usuário (pelo [](https://passwordreset.microsoftonline.com/) usuário ou pelo administrador), direcionar o usuário para aka.ms/sspr para que seus usuários possam ser habilitados para redefinir suas próprias senhas.
1. Se os usuários ainda estão enfrentando problemas, eles provavelmente serão **usuários sincronizados** com hash de senha ou **federados.** Isso significa que provavelmente há um problema com o serviço writeback de senha.