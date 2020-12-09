---
title: Entrar no Microsoft Edge automaticamente
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599437"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Entrar no Microsoft Edge automaticamente

O Microsoft Edge usa a conta padrão do sistema operacional para entrar automaticamente em um usuário de acordo com a configuração do dispositivo do usuário. 

Os cenários de cada tipo de configuração de dispositivo e seu processo de entrada dependente de usuário são descritos abaixo:

1. **O dispositivo é híbrido/AAD-J**: essa opção está disponível no Windows 10, no Windows de nível inferior e nas versões de servidor correspondentes. Os usuários são conectados automaticamente às suas contas do Azure Active Directory (AD).
2. **O dispositivo está associado ao domínio**: essa opção está disponível no Windows 10, no Windows de nível inferior e nas versões de servidor correspondentes. Por padrão, os usuários com contas de domínio não são conectados automaticamente; para habilitar a entrada automática, use a política **ConfigureOnPremisesAccountAutoSignIn** . Para habilitar a entrada automática para usuários com contas do Azure AD, considere o ingresso híbrido de seus dispositivos.
3. **A conta padrão do sistema operacional é uma conta da Microsoft**: essa opção está disponível no Windows 10 RS3 (versão 1709, Build 10.0.16299) e versões posteriores. O cenário provavelmente ocorrerá em dispositivos corporativos. No entanto, se a conta padrão do sistema operacional for uma conta da Microsoft, o Microsoft Edge entrará automaticamente no usuário com a conta da Microsoft.
 
 
