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
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950501"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Sua caixa de correio de arquivo morto está quase cheia

Se o usuário receber o aviso; **Sua caixa de correio de arquivo** morto está quase cheia ou você precisa aumentar o tamanho da caixa de correio de arquivo morto, aqui estão algumas dicas:

1. Se o usuário tiver uma licença do Plano 1 do Exchange Online, atualize para o **Plano 2** do Exchange Online para aumentar o tamanho de 50 GB para 100 GB.
1. Se o usuário já tiver atribuído um dos seguintes: Plano **2** do Exchange Online ou Um Plano 1 do Exchange Online com um complemento de Arquivamento do Exchange Online, use as etapas abaixo para habilitar o arquivamento de Expansão Automática:.
 
    1. [Conecte-se ao Powershell do Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Execute o seguinte commandlet para o usuário:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Execute o seguinte commandlet para confirmar se ele está habilitado para o usuário:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Para obter mais informações, consulte:

- [ Habilitar arquivamento ilimitado - Ajuda para Administradores - Microsoft 365 Compliance | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Limites do Exchange Online - Descrições de | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Atualizar para um plano de negócios | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

