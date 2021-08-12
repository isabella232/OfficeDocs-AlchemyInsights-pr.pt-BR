---
title: Read-Only mensagem de Manutenção ao tentar usar SharePoint ou OneDrive
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
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910532"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only mensagem de Manutenção ao tentar usar SharePoint ou OneDrive

Os usuários podem receber uma **mensagem Somente** leitura para Manutenção ao tentar usar SharePoint ou OneDrive para um dos seguintes cenários. 

-   Uma atividade de manutenção planejada ou ativa.  Verifique se eles estão navegando até o Centro [de Mensagens](https://portal.office.com/adminportal/home#/messagecenter).
-   Um incidente de serviço ativo de alta prioridade que pode estar ocorrendo. Verifique se há avisos/incidentes navegando para a [Saúde do Serviço.](https://portal.office.com/adminportal/home#/servicehealth)
-   Um cenário de recuperação automática secundária que pode estar acontecendo devido a eventos inesperados nos servidores que podem durar menos de 30 minutos. 
    
    Não há nenhuma central de mensagens ou postagens de Saúde do Serviço para essas pequenas recuperações, mas você deve voltar ao normal muito em breve.

Em poucas ocasiões, observamos que um dos três cenários listados acima foi a causa e o serviço foi restaurado, mas o cache do navegador dos usuários não foi limpo.

Tente limpar o cache do navegador antes de navegar para o site.

1. No navegador Microsoft Edge, selecione **Configurações** e, em seguida, **selecione Privacidade e Segurança.**
2. Em **Limpar navegação,** selecione **Escolher o que limpar**.
3. Selecione **Cookies e dados de site salvos** e selecione **Limpar**.

>[!Note] 
> Essas etapas podem ser diferentes ao usar outros navegadores, como o Mozilla Firefox ou o Google Chrome.

>[!Note] 
> Outra opção seria abrir seu site SharePoint ou OneDrive em uma nova janela InPrivate.