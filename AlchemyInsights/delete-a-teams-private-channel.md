---
title: Excluir um canal privado do Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431295"
---
# <a name="delete-a-teams-private-channel"></a>Excluir um canal privado do Teams

A Microsoft está ciente de um problema ao excluir um canal privado do Teams, caso você tenha Políticas de Retenção do SharePoint habilitadas para o site do SharePoint subjacente. A Microsoft está trabalhando em uma correção. Enquanto isso, você pode usar as seguintes soluções alternativas para excluir o canal privado:

**Exclua a coleção do Team/site da política de retenção do SharePoint.**

1. Vá para o portal de administração do Office 365 e selecione **Mostrar todos** no painel de navegação à esquerda.
2. Em **Centros de Administração**, vá para **Segurança e Conformidade** > **Prevenção de Perda de Dados** > **Política**.
3. Identifique qualquer política que se aplica aos sites do SharePoint, e modifique a política de modo que o site do SharePoint para o Team que contém o canal privado NÃO esteja incluído na política de retenção.
4. Salvar a política.
    Pode levar até 24 horas para as configurações de política terem efeito.
    Depois que o site tiver sido excluído, você poderá excluir o canal privado.  
    
Você ***pode*** ser capaz de excluir o canal privado usando o Microsoft Teams em seu dispositivo Android. 

Para informações relacionadas ao SharePoint, confira [Não é possível excluir itens no SharePoint Online ou no OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).