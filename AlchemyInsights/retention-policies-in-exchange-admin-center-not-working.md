---
title: Políticas de retenção no Centro de Administração do Exchange não estão funcionando
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952216"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Políticas de retenção no Centro de Administração do Exchange

Se você quiser que executemos verificações automatizadas para as configurações mencionadas abaixo, selecione o botão voltar <-- na parte superior desta página e insira o endereço de email do usuário que tenha problemas com políticas de retenção.

Se você tiver problemas com políticas de retenção no Centro de Administração do Exchange não se aplicando a caixas de correio ou itens que não se movem para a caixa de correio de arquivo morto, verifique o seguinte:

**Causas raiz:**

- **O Assistente de Pasta Gerenciada** não processou a caixa de correio do usuário. O Assistente de Pasta Gerenciada tenta processar todas as caixas de correio em sua organização baseada em nuvem uma vez a cada sete dias.

  **Solução:** Execute o Assistente de Pasta Gerenciada.

- **RetentionHold** foi **habilitado na** caixa de correio. Se a caixa de correio tiver sido colocada em um RetentionHold, a política de retenção na caixa de correio não será processada durante esse tempo.

  **Solução:** Verifique o status da configuração de Retenção e atualização conforme necessário. Para obter detalhes, consulte [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Observação:** Se uma caixa de correio for menor que 10 MB, o Assistente de Pasta Gerenciada não processará automaticamente a caixa de correio.
 
Para obter mais informações sobre políticas de retenção no Centro de Administração do Exchange, consulte:

- [Marcas e políticas de retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Aplicar uma política de retenção a caixas de correio](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ou Adicionar ou remover marcas de [retenção](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Como identificar o tipo de retenção de uma caixa de correio](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
