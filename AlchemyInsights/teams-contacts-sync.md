---
title: Sincronização de contatos do Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: efc1f29c6e2f76d763f2f8102db7e9f6afb1f1be
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327321"
---
# <a name="teams-contacts-sync"></a>Sincronização de contatos do Teams

Os contatos do Teams em sua organização usam o Active Directory e os contatos do Outlook adicionados à pasta padrão do usuário. Se os contatos não aparecerem no Microsoft Teams, tente o seguinte:

**Observação**: se as informações de um ou mais contatos foram atualizadas recentemente, pode levar até 48 horas para que os contatos sejam sincronizados.

1. Saia do Teams e reinicie. Verifique os contatos aparecem para Eliseu.
1. Limpe o cache no Teams:
    1. Navegue até **%appdata%\Microsoft\Teams**.
    1. Exclua os conteúdos da pasta.
    1. Reinicie o computador e Inicie o Teams.
1. Se o contato for do Outlook, certifique-se de adicioná-lo à Lista de contatos. No Outlook, na barra de endereço, selecione **Arquivo** e, em seguida, selecione **Adicionar aos Contatos**.
1. Certifique-se de que daria à Caixa de correio trocas de está hospedados online avatar (não local). Para saber mais, confira [Como o Exchange e o Microsoft Teams interagem](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
1. Certifique-se de que o número de telefone do contato seja adicionado às informações de contato.
1. Pesquise o email do contato na barra de pesquisa. Os contatos que você pode recuperar podem ser sincronizados com a Lista de Contatos.
