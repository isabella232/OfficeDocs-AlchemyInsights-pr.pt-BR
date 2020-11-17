---
title: Perguntas sobre como usar a ferramenta de implantação do Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086144"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Perguntas sobre como usar a ferramenta de implantação do Office (ODT)

Baixe a Ferramenta de Implantação de Office do [Centro de Download da Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Após baixar o arquivo, execute o arquivo executável de extração automática, que contém o executável da ferramenta de implantação do Office (setupodt.exe) e um arquivo de configuração de exemplo (configuration.xml).
  
 **Para excluir ou remover aplicativos da Microsoft 365 para produtos corporativos de computadores cliente:**
  
Ao instalar o Microsoft 365 aplicativos para empresas, você pode excluir produtos específicos. Para fazer isso, siga as etapas para instalar o Office com a ODT, mas inclua o elemento ExcludeApp no arquivo de configuração. Por exemplo, esse arquivo de configuração instala todos os aplicativos do Microsoft 365 para produtos corporativos, exceto o Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Visão geral da Ferramenta de Implantação do Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

