---
title: Trabalhando com iOS VPP Applications Rule Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083002"
---
# <a name="working-with-ios-vpp-applications"></a>Trabalhar com aplicativos VPP do iOS

Leia Como gerenciar aplicativos [iOS](https://docs.microsoft.com/intune/vpp-apps-ios) adquiridos por meio de um programa de compra de volume com Microsoft Intune para saber mais sobre recursos, restrições e etapas para usar o Programa de Compra de Volume da Apple e o suporte para ele em Microsoft Intune.
  
 **Problemas comuns:** "Eu atribuído um aplicativo VPP do iOS aos meus usuários, mas a instalação falhou."
  
- Isso pode acontecer se um único token VPP for usado em vários provedores de gerenciamento de dispositivo móvel. Os tokens VPP da Apple só podem ser usados com um provedor. Se você usou um token VPP com vários provedores, você deve carregar o token de novo no Intune.

- A instalação também poderá falhar se o número total de instalações exceder o número de licenças. Para exibir um relatório de uso para suas licenças, acesse a página Licenças de aplicativos de aplicativos móveis **do Intune.** \>  Para saber como recuperar licenças em uso, consulte [este artigo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
