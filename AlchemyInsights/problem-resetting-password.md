---
title: Problema ao redefinir senha
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039954"
---
# <a name="problems-resetting-password"></a>Problemas para redefinir senha

A seguir estão alguns dos problemas que você pode enfrentar ao redefinir a senha e as soluções possíveis:

**Estou tendo um problema com a redefinição de senha não abordada nas outras categorias**

- Verifique se você está autorizado a redefinir senhas. Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário. Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.
- Certifique-se de entender os requisitos de licenciamento:
    - Você deve ter pelo menos uma licença atribuída em sua organização
        - Usuários somente na nuvem - SKU pago Office 365 (O365) ou Azure AD Basic
        - Usuários na nuvem e/ou locais - Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
        - Para ler mais sobre os requisitos de licenciamento, consulte o artigo Requisitos de licenciamento para a redefinição de senha de [autoatendados do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Estou com problemas para testar a política de redefinição de senha que defina**

- Políticas aplicadas recentemente podem levar vários minutos para replicar em todos os data centers e pontos de extremidade. A distância física do data center também afetará a rapidez com que as alterações são aplicadas.
- Teste com um usuário final, não um administrador e piloto com um pequeno conjunto de usuários. As políticas configuradas no portal do Azure APLICAM-se SOMENTE aos usuários finais, não aos administradores. A Microsoft impõe uma política de redefinição de senha de dois portais padrão forte para qualquer função de administrador do Azure (Exemplo: Administrador Global, Administrador de Ajuda, Administrador de Senha etc.)
    - Saiba mais sobre [políticas para administradores.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Quero implantar a redefinição de senha, mas não quero que meus usuários registrem informações adicionais de segurança**

Preencher previamente dados para seus usuários para que eles não tenham que fazer isso! - Como administrador, você pode definir propriedades de telefone e email para seus usuários antes de fazer a redefinição de senha para sua organização. Você pode fazer isso usando uma API, PowerShell ou Azure AD Conexão. Mais informações aqui:
- [Implantando redefinição de senha sem exigir que os usuários se registrem](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Quais dados são usados pela redefinição de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**O botão de redefinição de senha está acinzentado**

Você não está autorizado a redefinir as senhas desse usuário. Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário. Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.

**Não vejo a folha de redefinição de senha**

Você não está autorizado a redefinir senhas. Somente administradores globais, de senha e de usuário podem redefinir senhas de usuário. Os administradores globais também podem redefinir as senhas de outro administrador privilegiado.

**Não vejo a folha de integração local na redefinição de senha**

- A folha de integração local só aparece em ambientes híbridos , o que significa que você está usando o writeback de senha para manipular as senhas do usuário local.
- Você não verá essa folha se:
    - Você não está usando writeback de senha
    - Há um problema com a instalação/conectividade do writeback de senha
    - Há um problema com sua instalação/conectividade do Azure AD Conexão
    - Para obter mais etapas de solução de problemas para problemas com o writeback de senha, consulte a seção [Solucionar problemas de writeback de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Não sei como redefinir a senha de um usuário**

1. Entre no portal do Azure como um administrador apropriado.
1. Vá para a folha Usuários e grupos, selecione **Todos os Usuários**.
1. Selecione um usuário na lista.
1. Para o usuário selecionado, selecione **Visão Geral** e, em seguida, na barra de comandos, clique em **Redefinir senha**.
1. Siga as instruções na tela.
    - Somente as redefinições realizadas por meio do portal do Azure suportam o writeback de senha.

**Redefini a senha de um usuário local do portal de administração Office 365 ou do aplicativo móvel Office 365, mas o usuário ainda não consegue entrar**

O Writeback de senha não é suportado neste portal. Redefinir a senha do usuário novamente no portal do Azure - portal.azure.com

