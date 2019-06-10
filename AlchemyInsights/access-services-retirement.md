---
title: Aposentadoria de serviços do Access
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769425"
---
# <a name="access-services-retirement"></a>Aposentadoria de serviços do Access

Como anunciamos originalmente no MC97576, em março de 2017, e continuamos a se comunicar nos serviços de acesso do ano passado estão sendo retirados do Office 365. A próxima fase desse processo será a remoção dos bancos de dados do Access Web que usam as listas do SharePoint como armazenamento de dados subjacente.

**Como isso me afeta?**

A partir de junho de 2019, implantaremos a criação de novos bancos de dados do Access no SharePoint Online e encerrará o serviço e todos os aplicativos restantes em abril de 2020.

**O que eu preciso fazer para se preparar para essa alteração?**

Recomendamos que você crie um plano de transição para os bancos de dados de acesso da sua organização. Os administradores podem usar o verificador de [aplicativos do Access do SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obter um inventário dos aplicativos do Access que os sites estão usando. 

Há várias maneiras de migrar os dados dos bancos de dados da Web do Access:

- Importando para um banco de dados de acesso local (. ACCDB) ou para um arquivo do Excel.
- Também recomendamos explorar o Microsoft PowerApps como uma plataforma alternativa para criar soluções de negócios sem código para dispositivos da Web e móveis.