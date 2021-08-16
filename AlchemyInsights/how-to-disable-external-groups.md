---
title: Como desabilitar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015608"
---
# <a name="how-to-disable-external-groups"></a>Como desabilitar grupos externos

Yammer de mensagens externas aplica-se Exchange regras de transporte (ETRs), um conjunto de controles proativos para impedir que as informações da empresa são compartilhadas. Para restringir os usuários de criar grupos externos, você precisa configurar uma regra de transporte Exchange (ETR) e configurar o Yammer para usar a regra de transporte Exchange para bloquear mensagens externas.
  
Depois de criar uma regra no Exchange Online de administração, siga estas etapas para definir o ETR a ser aplicado Yammer:
  
- Faça logon no Yammer como administrador verificado e, no centro de administração do **Yammer,** vá para C Conteúdo e **Segurança \> Configurações.**

- Em **Mensagens Externas,** selecione **Impor suas Exchange Online Exchange de Transporte (ETRs) em Yammer.**

- Escolha **Salvar**.

Para obter mais informações, consulte [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  