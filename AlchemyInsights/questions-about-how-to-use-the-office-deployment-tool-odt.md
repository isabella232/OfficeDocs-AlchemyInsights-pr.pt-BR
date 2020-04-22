---
title: Perguntas sobre como usar a ferramenta de implantação do Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698046"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Perguntas sobre como usar a ferramenta de implantação do Office (ODT)

Baixe a Ferramenta de Implantação de Office do [Centro de Download da Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Após baixar o arquivo, execute o arquivo executável de extração automática, que contém o executável da Ferramenta de Implantação do Office (setup.exe) e um arquivo de configuração de exemplo (configuration.xml).
  
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

[Visão geral da Ferramenta de Implantação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

