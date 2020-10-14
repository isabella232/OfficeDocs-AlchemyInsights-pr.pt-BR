---
title: Microsoft Teams-acesso de convidado
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: ee38dcb5f40ea16cea1b84b9b16e86b0f52f2d89
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48452216"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams-acesso de convidado

Se você precisar de ajuda para se comunicar com usuários fora da sua organização no Microsoft Teams, será necessário decidir se usará o [acesso de convidados ou o acesso externo (Federação)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)ou se você poderá usar ambos.

Certifique-se de [revisar as diferenças](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) para entender os recursos disponíveis para cada um deles.  Por exemplo, o acesso externo (Federação) permite comunicações 1:1, como chat e presença.  Os usuários federados não podem participar da colaboração do teams no entanto.  Se você quiser que um usuário externo ingresse e participe de conversas de canal de equipes ou compartilhar arquivos, precisará ativar o acesso de convidados.

**Opção 1: ativar o acesso de convidados** No centro de administração do Microsoft Teams, acesse [configurações do org Wide > acesso de convidados](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) e ative "permitir acesso de convidados no Teams".  Para um locatário com todas as outras configurações padrão, isso deve ser tudo o que você precisa fazer.  Para personalizar sua configuração de acesso de convidados, certifique-se de seguir todas as etapas na [lista de verificação de acesso de convidados](https://docs.microsoft.com/microsoftteams/guest-access-checklist). Após concluir, você precisará [aguardar até 24 horas](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) para que as configurações entrem em vigor.

Se você tiver certeza de que concluiu todas as etapas da lista de verificação e tiver sido mais de 24 horas, vá em frente e tente [Adicionar um convidado para sua equipe](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Para obter mais informações, incluindo vídeos explicativos, consulte [acesso de convidados no Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Opção 2: ativar o acesso externo (Federação)** Se você também quiser ativar o acesso externo (Federação), no centro de administração do Microsoft Teams, vá para [configurações de toda a organização > acesso externo](https://admin.teams.microsoft.com/company-wide-settings/external-communications) e ative "os usuários podem se comunicar com o Skype for Business e os usuários do Teams" e siga todas as etapas em [permitir que os usuários do Microsoft Teams conversem e se comuniquem com usuários em outra organização](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).
