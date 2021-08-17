---
title: Entre no Microsoft Edge automaticamente
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050682"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Entre no Microsoft Edge automaticamente

Microsoft Edge usa a conta padrão do sistema operacional para entrar automaticamente em um usuário de acordo com a configuração do dispositivo do usuário. 

Os cenários de cada tipo de configuração de dispositivo e seu processo de entrada dependente do usuário são descritos abaixo:

- **O dispositivo é híbrido/AAD-J**: essa opção está disponível em Windows 10, no nível inferior Windows e nas versões correspondentes do servidor. Os usuários são automaticamente assinados com suas Azure Active Directory (AD)contas.
- **O dispositivo é ingressado** em domínio : essa opção está disponível em Windows 10, no nível inferior Windows e nas versões correspondentes do servidor. Por padrão, os usuários com contas de domínio não são automaticamente assinados; para habilitar a assinatura automática para eles, use a **política ConfigureOnPremisesAccountAutoSignIn.** Para habilitar a entrada automática para usuários com contas do Azure AD, considere a junção híbrida em seus dispositivos.
- A conta padrão do sistema operacional é uma conta **da Microsoft**: essa opção está disponível no Windows 10 RS3 (versão 1709, build 10.0.16299) e versões posteriores. É improvável que o cenário ocorra em dispositivos corporativos. No entanto, se a conta padrão do sistema operacional for uma conta da Microsoft, Microsoft Edge entrará automaticamente no usuário com a conta da Microsoft.
 
 
