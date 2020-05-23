---
title: Solucionar problemas de autenticação SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264309"
---
# <a name="solving-smtp-authentication-issues"></a>Solucionar problemas de autenticação SMTP

Se você estiver obtendo erros 5.7.57 ou 5.7.3 ao tentar enviar um e-mail SMTP e autenticar com um cliente ou aplicativo, há algumas coisas que você deve verificar:

- O envio SMTP autenticado pode ser desabilitado no seu locatário ou na caixa de correio que você está tentando usar (verifique as duas configurações). Para saber mais, consulte [Habilite ou desabilite o envio SMTP autenticado](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Verifique se os [Padrões de segurança do Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) estão habilitados para o seu inquérito; se ativado, uma autenticação SMTP usando autenticação básica (também conhecida como herdada; isso usará o nome de usuário e a senha) falhará.
