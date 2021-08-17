---
title: Corrigir política de locatário (substituição de ação)
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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896063"
---
# <a name="fix-tenant-policy-action-override"></a>Corrigir política de locatário (substituição de ação)

Uma de suas políticas anti-spam afetou essa mensagem. Para revisar as políticas, faça as seguintes etapas:

1. No portal Microsoft 365 Defender , acesse Email & Políticas de Colaboração & Políticas de Ameaças de Regras <https://security.microsoft.com/>  \>  \>  \> **Anti-spam** na **seção** Políticas.

   Para ir diretamente à página de **Políticas antispam**, use <https://security.microsoft.com/antispam>.

2. Na página **Políticas anti-spam,** selecione a política clicando no nome da política (**Tipo** é Política **anti-spam** personalizada ou **Nome** é Política de entrada **Anti-Spam (Padrão)**).
3. No sobremenu de detalhes exibido, selecione **Editar ações** na **seção** Ações.
4. Na seção **Ações de mensagem,** revise os vereditos para **Spam,** **spam** de alta confiança, phishing e **phishing** de alta confiança para ver se algum dos seguintes valores está selecionado: 
   - **Adicionar cabeçalho X**
   - **Preceder a linha do assunto com texto**
   - **Redirecionar mensagem para endereço de email**
   - **Excluir mensagem**
   - **Nenhuma ação**

   É possível que as configurações **Padrão aplicadas** a todos os clientes Proteção do Exchange Online afetaram a mensagem.

Para obter mais informações, consulte [Configure as políticas de anti-spam no EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
