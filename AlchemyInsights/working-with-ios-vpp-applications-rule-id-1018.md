---
title: Trabalhando com iOS VPP 1018 de Id de regra de aplicativos
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917484"
---
# <a name="working-with-ios-vpp-applications"></a>Trabalhando com iOS VPP aplicativos

Leia [como gerenciar aplicativos de iOS adquiridos por meio de um programa de compra do volume com Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para saber mais sobre recursos, restrições e etapas para fazer uso do programa de compra de Volume da Apple e o suporte para ele no Microsoft Intune. 
  
 **Problemas comuns:** "Eu atribuída a um aplicativo VPP iOS a meus usuários, mas a instalação falhou." 
  
- Isso pode acontecer se um único token VPP for usado em vários provedores de gerenciamento de dispositivo móvel. Tokens VPP da Apple só podem ser usados com um provedor. Se você tiver usado um token VPP com vários provedores, você deve reenvie o token para Intune.
    
- A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para exibir um relatório de uso de suas licenças, vá para o **Intune Mobile apps** \> página **licenças de aplicativo** . Para saber como recuperar licenças em uso, consulte [neste artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

