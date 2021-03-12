---
title: Exemplo da política anti-phishing do Microsoft Defender para Office 365
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735700"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Exemplo da política anti-phishing do Microsoft Defender para Office 365

Essas configurações habilitam uma política chamada *Domínio e CEO.* Essa política fornece proteção de usuário e domínio contra representação e aplica a política a todos os emails recebidos pelos usuários no domínio. Primeiro, adicione as seguintes informações para criar a política:

- **Nome**: Domínio e CEO **Descrição**: Garante que o CEO e seu domínio não estão sendo personificados.
  **Aplicado a**: Selecione **O domínio do destinatário é**. Em **Qualquer um desses**, selecione **Escolher** e selecione um domínio. Selecione **+ Adicionar**. Marque a caixa de seleção ao lado do nome do domínio na lista *(por* exemplo, contoso.com ), e selecione **Adicionar**. Selecione **Concluído**.
- Após a criação da política, você pode ajustar a política usando as seguintes opções:
  - **Adicionar usuários para proteger:** Para este exemplo, adicione o endereço de email do CEO, no mínimo.
  - **Adicionar domínios para proteger**: Adicione o domínio organizacional que inclui o escritório do CEO.
  - **Escolha ações**: Para **se o email** for enviado por um usuário personificado, selecione Redirecionar mensagem para outro endereço de **email** e insira o endereço de email do administrador de segurança *(por* exemplo, securityadmin@contoso.com ). For **If email is sent by an impersonated domain**, select Quarantine the **message**.
  - **Inteligência de caixa** de correio : Por padrão, essa opção é selecionada quando você cria uma nova política anti-phishing. Deixe essa configuração **Ativada** para obter melhores resultados.
  - **Adicionar senders e domínios confiáveis:** Para este exemplo, não defina nenhuma substituição.
- Depois de revisar suas configurações, selecione **Criar essa política** ou **Salvar**, conforme apropriado.

Para saber mais, confira [Políticas anti-phishing no Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
