---
title: Somente leitura para mensagem de manutenção ao tentar usar o SharePoint ou o OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670820"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Somente leitura para mensagem de manutenção ao tentar usar o SharePoint ou o OneDrive

Os usuários podem receber uma mensagem **somente leitura para manutenção** ao tentar usar o SharePoint ou o onedrive para um dos cenários a seguir. 

-   Uma atividade de manutenção planejada ou ativa.  Verifique se eles navegam para o [centro de mensagens](https://portal.office.com/adminportal/home#/messagecenter).
-   Um incidente de serviço ativo de alta prioridade que pode ocorrer. Verifique se há avisos/incidentes navegando até a [integridade do serviço](https://portal.office.com/adminportal/home#/servicehealth).
-   Um cenário de recuperação de reparo automático secundário que pode ocorrer devido a qualquer evento inesperado nos servidores que podem durar menos de 30 min. 
    
    Não há postagens do centro de mensagens ou da integridade do serviço para essas pequenas recuperações, mas você deve voltar para o normal em breve.

Em muito poucas ocasiões observamos que um dos três cenários listados acima tem sido a causa, e o serviço foi restaurado, mas o cache do navegador do usuário não foi apagado.

Tente limpar o cache do navegador antes de navegar até o site.

1. No navegador Microsoft Edge, selecione **configurações**e, em seguida, selecione **privacidade e segurança**.
2. Em **limpar navegação**, selecione **escolher o que limpar**.
3. Selecione **cookies e dados de sites salvos**e selecione **limpar**.

>[!Note] 
> Essas etapas podem diferir ao usar outros navegadores, como Mozilla Firefox ou Google Chrome.

>[!Note] 
> Outra opção seria abrir seu site do SharePoint ou o OneDrive em uma nova janela InPrivate.