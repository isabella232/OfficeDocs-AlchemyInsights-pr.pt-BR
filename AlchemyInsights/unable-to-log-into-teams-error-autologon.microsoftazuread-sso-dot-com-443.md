---
title: Não é possível entrar no Teams devido ao erro autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038388"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Não é possível entrar no Teams devido ao erro autologon.microsoftazuread-sso dot com:443

Se o SSO Contínuo estiver ativado como a autenticação do O365, talvez seja necessário adicionar a URL "autologon.microsoftazuread-sso.com" aos Sites da Intranet.  Se ela tiver sido adicionada anteriormente aos Sites Confiáveis e o SSO Contínuo estiver em uso, ela deve ser removida dos Sites Confiáveis.

Examine a [lista de verificação de solução de problemas de SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Siga estas etapas para adicionar uma URL à lista de Sites da Intranet:

1. Abra o Internet Explorer clicando no botão **Iniciar**. Na caixa de pesquisa, digite Internet Explorer e, em seguida, na lista de resultados, clique em **Internet Explorer**.
2. Clique em **Ferramentas** e em **Opções da Internet**.
3. Clique na guia **Segurança**.
4. Agora, clique em **Sites da intranet local** e, em seguida, clique no botão **Sites** e depois no botão **Avançado**.
5. Insira a URL do site e clique em **Adicionar**.
6. Quando terminar, clique em **Fechar**.

Para saber mais, confira a [Documentação para a implantação do SSO Contínuo no O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inclui o processo baseado em políticas para adicionar uma URL aos sites da intranet na etapa 3).
