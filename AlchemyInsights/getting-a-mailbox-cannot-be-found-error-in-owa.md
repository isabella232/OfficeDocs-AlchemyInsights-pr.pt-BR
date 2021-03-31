---
title: 126 Não é possível encontrar erro ao obter uma caixa de correio no OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426650"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Obter uma caixa de correio não encontrada erro no Outlook na Web?

Se você estiver usando o Outlook na Web e receber uma Caixa de Correio não foi encontrada por erro, **a** conta que você usou para se conectar ao Outlook na Web não tem uma licença do Exchange Online e, portanto, nenhuma caixa de correio está associada à conta. O administrador pode atribuir uma licença à sua conta seguindo estas etapas:

1. Abra o Centro de administração do  [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e vá para Usuários ativos na seção **Usuários** e selecione o usuário que está vendo o erro.

2. Na página de usuário aberta, vá para a seção  Licenças e **Aplicativos,** selecione o valor local apropriado e atribua uma licença que contenha o Exchange Online (expanda a licença para ver seus detalhes). Quando terminar, clique em **Salvar alterações**.

Em alguns casos, se a licença já estiver atribuída a uma conta de usuário, remover e reatribuir a licença ajuda a resolver o problema e a provisioná-la corretamente no sistema: 

- Verifique se suas assinaturas do M365 Exchange Online (e outras, se você tiver alguma) estão atuais e não expiraram recentemente.

Depois de certificar-se de que sua assinatura não expirou e que uma licença válida foi atribuída à conta de usuário, pode levar até 24 horas para que a licença seja provisionada, portanto, talvez seja necessário aguardar a resolução do problema. Para obter mais informações, [consulte Atribuir e gerenciar licenças.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)