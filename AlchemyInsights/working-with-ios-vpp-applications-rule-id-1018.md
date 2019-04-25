---
title: Trabalhando com o ID de regra de aplicativos VPP iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420472"
---
# <a name="working-with-ios-vpp-applications"></a>Trabalhar com aplicativos VPP do iOS

Leia [como gerenciar aplicativos Ios adquiridos por meio de um programa de compra de volume com o Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para saber mais sobre recursos, restrições e etapas para usar o Apple Volume Purchase Program e o suporte para ele no Microsoft Intune. 
  
 **Problemas comuns:** "Atribuí um aplicativo VPP iOS a meus usuários, mas a instalação falhou." 
  
- Isso pode acontecer quando um único token VPP é usado em vários provedores de gerenciamento de dispositivos móveis. Os tokens de VPP da Apple só podem ser usados com um provedor. Se você usou um token VPP com vários provedores, você deve recarregar o token para o Intune.
    
- A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para exibir um relatório de uso para suas licenças, acesse a página **licenças** de aplicativos **móveis** \> do Intune. Para saber como recuperar licenças em uso, consulte [Este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

