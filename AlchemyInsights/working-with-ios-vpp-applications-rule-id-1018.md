---
title: Trabalhando com o ID de regra de aplicativos VPP iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557968"
---
# <a name="working-with-ios-vpp-applications"></a>Trabalhar com aplicativos VPP do iOS

Leia [como gerenciar aplicativos Ios adquiridos por meio de um programa de compra de volume com o Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) para saber mais sobre recursos, restrições e etapas para usar o Apple Volume Purchase Program e o suporte para ele no Microsoft Intune.
  
 **Problemas comuns:** "Atribuí um aplicativo VPP iOS a meus usuários, mas a instalação falhou."
  
- Isso pode acontecer quando um único token VPP é usado em vários provedores de gerenciamento de dispositivos móveis. Os tokens de VPP da Apple só podem ser usados com um provedor. Se você usou um token VPP com vários provedores, você deve recarregar o token para o Intune.

- A instalação também pode falhar se o número total de instalações exceder o número de licenças. Para exibir um relatório de uso para suas licenças, acesse a página **licenças** de aplicativos **móveis** \> do Intune. Para saber como recuperar licenças em uso, consulte [Este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
