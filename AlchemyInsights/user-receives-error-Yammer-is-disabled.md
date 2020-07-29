---
title: O usuário recebe o erro AADSTS7000112 o Yammer está desabilitado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157258"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>O usuário recebe o erro AADSTS7000112 o Yammer está desabilitado

Se você receber a mensagem de erro "AADSTS7000112: aplicativo '00000005-0000-0ff1-ce00-000000000000' "(Yammer) está desabilitado", há um problema com a entidade de serviço no Azure AD. Um administrador pode ter desabilitado a entidade de serviço para bloquear o acesso ao Yammer.

Desabilitar a entidade de serviço não é recomendável e pode causar problemas adicionais. Para obter mais informações sobre a abordagem adequada para bloquear o acesso do usuário ao Yammer, confira [Desativar o acesso ao Yammer para usuários do Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Para corrigir esse problema no portal do Azure e restaurar o acesso do usuário ao Yammer:

1.  Abra a página do Azure Active Directory e selecione **Aplicativos corporativos** em **Gerenciar** no painel de navegação à esquerda.
3.  Digite **Office 365 Yammer** na caixa de pesquisa e selecione o nome do aplicativo para abrir as configurações.
4.  Selecione **Propriedades** em **Gerenciar** no painel de navegação à esquerda.
5.  Defina o valor da **Habilitada para que os usuários entrem?** para**Sim**e selecione **Salvar**.
6.  Entre no Yammer novamente. Talvez seja necessário limpar os cookies.

Como alternativa, execute os comandos do PowerShell para definir o valor. Para saber mais, confira o artigo [Erro "Infelizmente, você está com problemas para entrar" quando você clica no bloco do Yammer no Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 