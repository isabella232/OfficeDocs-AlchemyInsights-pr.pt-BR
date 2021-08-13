---
title: Configurar regras para responder a emails de entrada
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "7254"
ms.openlocfilehash: 3164959f33a42e518002e4c222a344d4f638d17a32a4959db2f903ce5cb14d81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53915611"
---
# <a name="set-up-rules-to-reply-to-incoming-emails"></a>Configurar regras para responder a emails de entrada

Use as etapas a seguir para criar um modelo para responder a mensagens e, em seguida, configurar um Outlook para responder a cada mensagem recebida.

1. Em Outlook, crie uma nova mensagem de email e insira um assunto e um corpo de mensagem para seu modelo fora do escritório.
2. Selecione **Arquivo > Salvar como**.
3. Na caixa de diálogo Salvar  **como,** na lista de opções Salvar como tipo, selecione Outlook **Modelo (*.oft).** Dê a ele um nome apropriado e clique em **Salvar**.
4. Selecione o **arquivo Gerenciar** Regras  >  **& Alertas**.
5. Na caixa de diálogo Regras e **Alertas,** na guia Regras de **Email,** clique em **Nova Regra**.
6. Na caixa **de diálogo Assistente** de Regras, em Iniciar de **uma** regra em branco, selecione **Aplicar regra** nas mensagens que recebo e clique em **Próximo**.
7. Para a condição, selecione **enviado somente para mim** e clique em **Próximo**.
8. Para a ação, selecione **responder usando um modelo específico** e, no painel inferior, clique em um modelo **específico.**
9. Na caixa **de diálogo Selecionar um Modelo** de Resposta, no drop-down Look **In,** selecione Modelos de Usuário **no Sistema de Arquivos**. Escolha o modelo salvo anteriormente e clique em **Abrir**.
10. No painel inferior da caixa de diálogo, você verá que o arquivo de modelo está inserido. Clique **em Concluir** para fechar o assistente e retornar à caixa de diálogo Regras e **Alertas.** Observe a regra **recém-criada enviada apenas para** mim. Clique em **OK**.
