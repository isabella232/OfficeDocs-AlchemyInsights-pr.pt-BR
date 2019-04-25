---
title: Perguntas sobre como usar a ferramenta de implantação do Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371756"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Perguntas sobre como usar a ferramenta de implantação do Office (ODT)

Baixe a Ferramenta de Implantação de Office do [Centro de Download da Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Após baixar o arquivo, execute o arquivo executável de extração automática, que contém o executável da Ferramenta de Implantação do Office (setup.exe) e um arquivo de configuração de exemplo (configuration.xml).
  
 **Para excluir ou remover produtos do Office 365 proPlus de computadores cliente:**
  
Ao instalar o Office 365 ProPlus, você pode excluir produtos específicos. Para fazer isso, siga as etapas para instalar o Office com a ODT, mas inclua o elemento ExcludeApp no arquivo de configuração. Por exemplo, esse arquivo de configuração instala todos os produtos do Office 365 ProPlus exceto o Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Visão geral da Ferramenta de Implantação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

