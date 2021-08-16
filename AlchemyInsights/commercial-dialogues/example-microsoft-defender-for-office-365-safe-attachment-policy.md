---
title: Exemplo do Microsoft Defender para Office 365 Cofre de anexos
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988283"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exemplo do Microsoft Defender para Office 365 Cofre de anexos

Essas configurações habilitam uma política chamada *Sem atrasos* que entrega mensagens imediatamente e, em seguida, reatta anexos depois que eles são verificados:

- **Nome**: Sem atrasos
- **Descrição**: entrega mensagens imediatamente e reatta anexos após a verificação.
- **Resposta**: selecione a **opção Entrega** Dinâmica. Para obter mais informações, consulte [Dynamic Delivery in Cofre Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Seção Anexo de** redirecionamento: selecione a opção Habilitar redirecionamento **e** insira o endereço de Microsoft 365 email do seu administrador global, administrador de segurança ou analista de segurança que investigará anexos mal-intencionados.
- **Seção Aplicado a:** Selecione **O domínio do destinatário é** e selecione seu domínio. Selecione **adicionar** e, em seguida, selecione **OK**. Depois de terminar, selecione **Salvar**.

Para saber mais, consulte [Cofre Anexos no Microsoft Defender para Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
