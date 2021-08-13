---
title: Aposentadoria dos serviços do Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938683"
---
# <a name="access-services-retirement"></a>Aposentadoria dos serviços do Access

Como anunciamos originalmente no MC97576, em março de 2017, e continuamos a se comunicar no último ano Serviços do Access estão sendo retirados. A próxima fase nesse processo será a remoção dos Bancos de Dados web do Access que usam SharePoint como seu armazenamento de dados subjacente.

**Como isso me afeta?**

A partir de junho de 2019, interromperemos a criação de novos bancos de dados do Access no SharePoint Online e desligaremos o serviço e todos os aplicativos restantes até abril de 2020.

**O que preciso fazer para me preparar para essa mudança?**

Recomendamos que você crie um plano de transição para os bancos de dados web do Access da sua organização. Os administradores podem usar o [SharePoint de aplicativos](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) do Access para obter um inventário dos aplicativos do Access que os sites estão usando.

Há várias maneiras de migrar dados de bancos de dados da Web do Access:

- Importando para um banco de dados local do Access (. ACCDB) ou para um arquivo Excel.
- Também recomendamos explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções comerciais sem código para dispositivos web e móveis.