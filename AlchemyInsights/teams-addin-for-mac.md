---
title: Complemento do Teams para Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940663"
---
# <a name="teams-add-in-for-mac"></a>Complemento do Teams para Mac

Para solucionar os problemas de um complemento do Teams ausente para os usuários do sistema operacional Mac, siga estas etapas:

**Passo 1:** se você tiver o Hybrid Exchange On Premises (2016 CU3 ou posterior necessário), utilize a ferramenta Test-HMA.ps1 para confirmar se a Autenticação Hybrid Modern está configurada corretamente. Para mais informações, consulte [Validando a configuração da Autenticação Hybrid Modern para Outlook para iOS e Android](https://aka.ms/TestHMAEAS).  

**Note** Use o formato de endereço UPN (por exemplo, [username@contoso.com](mailto:username@contoso.com)), não domínio\nome do usuário Faça isso até mesmo para os usuários com caixas de correio no Exchange Online.

**Passo 2:** Peça ao usuário que vá até **Ferramentas** > **Contas**... ,no Outlook para Mac, para encontrar e selecionar a conta. Confirme se o nome do usuário listado está no formato UPN (por exemplo,, [username@contoso.com](mailto:username@contoso.com)).

**Passo 3:** Confirme se o usuário possui uma licença do Microsoft Teams. O usuário deve estar utilizando a assinatura do Office 365 para Mac, versão 16.24 ou posterior.