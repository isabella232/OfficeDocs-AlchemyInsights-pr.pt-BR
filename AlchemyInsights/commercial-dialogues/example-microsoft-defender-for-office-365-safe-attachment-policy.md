---
title: Exemplo da política de Anexo Seguro do Microsoft Defender para Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735371"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exemplo da política de Anexo Seguro do Microsoft Defender para Office 365

Essas configurações habilitam uma política chamada *Sem atrasos* que entrega mensagens imediatamente e, em seguida, reatta anexos depois que eles são verificados:

- **Nome**: Sem atrasos
- **Descrição**: entrega mensagens imediatamente e reatta anexos após a verificação.
- **Resposta**: selecione a **opção Entrega** Dinâmica. Para obter mais informações, consulte [Entrega Dinâmica em Políticas de Anexos Seguros.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Seção Anexo de** redirecionamento: selecione a opção Habilitar redirecionamento **e** insira o endereço de email do administrador global do Microsoft 365, administrador de segurança ou analista de segurança que investigará anexos mal-intencionados.
- **Seção Aplicado a:** Selecione **O domínio do destinatário é** e selecione seu domínio. Selecione **adicionar** e, em seguida, selecione **OK**. Depois de terminar, selecione **Salvar**.

Para saber mais, confira [Anexos Seguros no Microsoft Defender para Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
