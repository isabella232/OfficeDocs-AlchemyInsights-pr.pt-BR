---
title: Correção de aplicativos do Microsoft 365 Não foi conseguindo encontrar licenças do office associadas a mensagem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816476"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Corrigir a mensagem de aplicativos do Microsoft 365 "Não foi difícil encontrar licenças do office associadas"

Se você receber essa mensagem, tente o seguinte:

1. Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando o acesso à Internet para aplicativos do Microsoft 365. Consulte URLs e intervalos de [endereços IP do Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Remova e [reatribua a licença do Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) para o usuário afetado. 
3. Abra um aplicativo do Office [e saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de qualquer conta de usuário existente.
4. Vá para Configurações do Windows > **Contas** Email & contas e remova todas as contas de  >  trabalho, exceto a conta afetada.
5. Vá para Configurações do Windows > **Contas Acessar** trabalho ou escola e desconecte todas as contas de  >  trabalho, exceto a conta afetada.
6. Reinicie o estado de ativação do Office. [Saiba como](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Entre usando](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) a conta de usuário afetada.

Para obter soluções adicionais de solução de problemas, consulte [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).