---
title: Sua caixa de correio de arquivo morto está quase cheia
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046740"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Sua caixa de correio de arquivo morto está quase cheia

Se o usuário receber o aviso; **Sua caixa de correio de arquivo** morto está quase cheia ou você precisa aumentar o tamanho da caixa de correio de arquivo morto, aqui estão algumas dicas:

1. Se o usuário tiver uma Exchange Online Plano 1, atualize para Exchange Online licença do **Plano 2** para aumentar o tamanho de 50 GB para 100 GB.
1. Se o usuário já tiver atribuído um dos seguintes: **Exchange Online Plano 2** ou um plano 1 Exchange Online com um complemento Arquivamento do Exchange Online, use as etapas abaixo para habilitar o arquivamento de Expansão Automática:.
 
    1. [Conexão para Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Execute o seguinte commandlet para o usuário:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Execute o seguinte commandlet para confirmar se ele está habilitado para o usuário:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Para saber mais, veja:

- [Habilitar arquivamento ilimitado - Ajuda do administrador - Microsoft 365 conformidade | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online limites - Descrições de serviço | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Atualizar para um plano de negócios | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

