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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="748a4-102">Perguntas sobre como usar a ferramenta de implantação do Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="748a4-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="748a4-103">Baixe a Ferramenta de Implantação de Office do [Centro de Download da Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="748a4-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="748a4-104">Após baixar o arquivo, execute o arquivo executável de extração automática, que contém o executável da Ferramenta de Implantação do Office (setup.exe) e um arquivo de configuração de exemplo (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="748a4-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="748a4-105">**Para excluir ou remover aplicativos da Microsoft 365 para produtos corporativos de computadores cliente:**</span><span class="sxs-lookup"><span data-stu-id="748a4-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="748a4-106">Ao instalar o Microsoft 365 aplicativos para empresas, você pode excluir produtos específicos.</span><span class="sxs-lookup"><span data-stu-id="748a4-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="748a4-107">Para fazer isso, siga as etapas para instalar o Office com a ODT, mas inclua o elemento ExcludeApp no arquivo de configuração.</span><span class="sxs-lookup"><span data-stu-id="748a4-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="748a4-108">Por exemplo, esse arquivo de configuração instala todos os aplicativos do Microsoft 365 para produtos corporativos, exceto o Publisher:</span><span class="sxs-lookup"><span data-stu-id="748a4-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="748a4-109">Visão geral da Ferramenta de Implantação do Office</span><span class="sxs-lookup"><span data-stu-id="748a4-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

