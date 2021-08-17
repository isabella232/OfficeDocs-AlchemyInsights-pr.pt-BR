---
title: O que fazer se os recursos do Azure não funcionarem corretamente no Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117076"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>O que fazer se os recursos do Azure não funcionarem corretamente no Microsoft Edge

Microsoft Edge [problemas](https://go.microsoft.com/fwlink/?linkid=2140608) conhecidos relacionados a zonas de segurança e podem afetar como os usuários do Azure fazem logoff no Windows Admin Center. Se você estiver com problemas para usar recursos do Azure com Microsoft Edge, experimente as seguintes etapas:

1. No menu **Iniciar,** pesquise opções **da Internet** e selecione-a.
2. Na caixa de diálogo Propriedades da **Internet,** vá para a **guia** Segurança.
3. Selecione a **zona Sites Confiáveis** e selecione o **botão Sites.**
4. Na caixa **de diálogo Sites confiáveis,** adicione a URL do gateway e e, em [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) seguida, selecione **Fechar**.
5. Na caixa de diálogo Propriedades da **Internet,** vá para a **guia** Privacidade.
6. Na seção **Bloqueador pop-up,** selecione **Configurações**. Na caixa de diálogo que é aberta, adicione sua URL de gateway, bem [https://login.microsoftonline.com](https://login.microsoftonline.com) como e , e selecione [https://login.live.com](https://login.live.com) **Fechar**.
