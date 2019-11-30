---
title: Corrigir aplicativos do Office não foi possível localizar a mensagem associada ao Office licenses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627906"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Corrigindo a mensagem "não foi possível encontrar licenças do Office associadas" no Office apps

Se você receber essa mensagem, tente o seguinte:

1. Verifique o firewall, o software antivírus e as configurações de proxy para confirmar que eles não estão bloqueando o acesso à Internet para os aplicativos do Office. Confira [URLs e intervalos de endereços IP do Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Remova e [reatribua a licença do Office](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) para o usuário afetado. 
3. Abra um aplicativo do Office e [saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de qualquer conta de usuário existente.
4. Vá para configurações do Windows > **contas** > de**email & contas**e remova todas as contas de trabalho, exceto a conta afetada.
5. Vá para configurações do Windows > acessar **contas** > de**trabalho ou escola**e desconectar todas as contas de trabalho, exceto a conta afetada.
6. Redefina o estado de ativação do Office. [Saiba como](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Entre](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.

Para soluções de solução de problemas adicionais, confira o artigo não [licenciado e erros de ativação no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).