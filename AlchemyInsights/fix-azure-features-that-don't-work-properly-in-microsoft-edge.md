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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576337"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>O que fazer se os recursos do Azure não funcionarem corretamente no Microsoft Edge

O Microsoft Edge tem [problemas conhecidos](https://go.microsoft.com/fwlink/?linkid=2140608) relacionados às zonas de segurança e pode afetar como os usuários do Azure fazem logon no centro de administração do Windows. Se você estiver tendo problemas para usar os recursos do Azure com o Microsoft Edge, tente as seguintes etapas:

1. No menu **Iniciar** , procure opções da **Internet** e selecione-a.
2. Na caixa de diálogo **Propriedades da Internet** , vá para a guia **segurança** .
3. Selecione a zona **sites confiáveis** e, em seguida, selecione o botão **sites** .
4. Na caixa de diálogo **sites confiáveis** , adicione sua URL de gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e [https://login.live.com](https://login.live.com) , em seguida, selecione **fechar**.
5. Na caixa de diálogo **Propriedades da Internet** , vá para a guia **privacidade** .
6. Na seção **bloqueador de pop-ups** , selecione **configurações**. Na caixa de diálogo que é aberta, adicione sua URL de gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e [https://login.live.com](https://login.live.com) , em seguida, selecione **Fechar**.
