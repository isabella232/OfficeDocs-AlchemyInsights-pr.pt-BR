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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398717"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Entrar no Microsoft Edge automaticamente

O Microsoft Edge usa a conta padrão do sistema operacional para entrar automaticamente em um usuário de acordo com a configuração do dispositivo do usuário. 

Os cenários de cada tipo de configuração de dispositivo e seu processo de entrada dependente do usuário são descritos abaixo:

- **O dispositivo é híbrido/AAD-J**: essa opção está disponível no Windows 10, no Windows de nível inferior e nas versões de servidor correspondentes. Os usuários são automaticamente assinados com suas contas do Azure Active Directory (AD).
- **O dispositivo é ingressado** no domínio : essa opção está disponível no Windows 10, no Windows de nível inferior e nas versões de servidor correspondentes. Por padrão, os usuários com contas de domínio não são automaticamente assinados; para habilitar a assinatura automática para eles, use a **política ConfigureOnPremisesAccountAutoSignIn.** Para habilitar a entrada automática para usuários com contas do Azure AD, considere a junção híbrida em seus dispositivos.
- A conta padrão do sistema operacional é uma conta **da Microsoft**: essa opção está disponível no Windows 10 RS3 (versão 1709, build 10.0.16299) e versões posteriores. É improvável que o cenário ocorra em dispositivos corporativos. No entanto, se a conta padrão do sistema operacional for uma conta da Microsoft, o Microsoft Edge entrará automaticamente no usuário com a conta da Microsoft.
 
 
