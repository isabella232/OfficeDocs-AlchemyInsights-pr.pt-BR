---
title: Correção Microsoft 365 aplicativos Não foi necessário encontrar licenças do office associadas a mensagem
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
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069592"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Corrigir a Microsoft 365 aplicativos "Não foi consegui encontrar licenças do office associadas" mensagem

Se você receber essa mensagem, tente o seguinte:

1. Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando o acesso à Internet para Microsoft 365 aplicativos. Consulte [Microsoft 365 URLs e intervalos de endereços IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Remova e [reatribua Office licença do](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) usuário afetado. 
3. Abra um Aplicativo do Office [e saia de](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) qualquer conta de usuário existente.
4. Vá para Windows Configurações > **Contas Email**& contas e remova todas as contas de  >  trabalho, exceto a conta afetada.
5. Vá para Windows Configurações > **Contas**  >  **Acessar trabalho ou escola** e desconecte todas as contas de trabalho, exceto a conta afetada.
6. Reinicie o estado de ativação do Office. [Saiba como](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Entre usando](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) a conta de usuário afetada.

Para obter soluções adicionais de solução de problemas, consulte [Product and activation errors](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)in Office .