---
title: O que fazer se os recursos do Azure não funcionarem corretamente no Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950319"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>O que fazer se os recursos do Azure não funcionarem corretamente no Microsoft Edge

O Microsoft Edge tem problemas conhecidos relacionados a zonas de segurança que podem afetar o modo como os usuários do Azure fazem logon no Windows Admin Center. Confira mais informações em [Problemas conhecidos do Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Se você estiver tendo problemas para usar os recursos do Azure com o Microsoft Edge, tente o seguinte:

1. No menu Iniciar, na barra de **Pesquisa**, digite **Opções da Internet** e selecione-o.
1. Em **Propriedades da Internet**, selecione a guia **Segurança**.
1. Selecione **Sites confiáveis** e, em seguida, **Sites**.
1. Adicione o seu URL de gateway, bem como <https://login.microsoftonline.com> e <https://login.live.com> e selecione **Fechar**.
1. Em **Propriedades da Internet**, selecione a guia **Privacidade**.
1. Na seção Bloqueador de pop-ups, selecione **Configurações**. Adicione o seu URL de gateway, bem como <https://login.microsoftonline.com> e <https://login.live.com> e, em seguida, selecione **Fechar**.