---
title: Complemento do Teams para Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617032"
---
# <a name="teams-add-in-for-mac"></a>Complemento do Teams para Mac

Para solucionar os problemas de um complemento do Teams ausente para os usuários do sistema operacional Mac, siga estas etapas:

**Passo 1:** se você tiver o Hybrid Exchange On Premises (2016 CU3 ou posterior necessário), utilize a ferramenta Test-HMA.ps1 para confirmar se a Autenticação Hybrid Modern está configurada corretamente. Para mais informações, consulte [Validando a configuração da Autenticação Hybrid Modern para Outlook para iOS e Android](https://aka.ms/AA980zq).  

**Note** Use o formato de endereço UPN (por exemplo, [username@contoso.com](mailto:username@contoso.com)), não domínio\nome do usuário Faça isso até mesmo para os usuários com caixas de correio no Exchange Online.

**Passo 2:** Peça ao usuário que vá até **Ferramentas** > **Contas**... ,no Outlook para Mac, para encontrar e selecionar a conta. Confirme se o nome do usuário listado está no formato UPN (por exemplo,, [username@contoso.com](mailto:username@contoso.com)).

**Passo 3:** Confirme se o usuário possui uma licença do Microsoft Teams. O usuário deve estar utilizando a assinatura do Office 365 para Mac, versão 16.24 ou posterior.