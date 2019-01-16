---
title: Usando a ferramenta de implantação do Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275022"
---
# <a name="using-the-office-deployment-tool-odt"></a>Usando a ferramenta de implantação do Office (ODT)

Você pode usar a ferramenta de implantação do Office (ODT) para implantar o Office 365 versões do Office. A ferramenta de implantação do Office (setup.exe) é executada a partir da linha de comando e usa um arquivo XML de configuração para determinar quais configurações a serem aplicadas ao implantar o Office.
  
1. Baixe a versão mais recente da ferramenta de implantação do Office a partir do [Centro de Download da Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Use a [Ferramenta de personalização do Office (OCT)](https://config.office.com) para selecionar suas preferências de implantação e criar o arquivo XML de configuração. Exporte o arquivo de configuração e colocá-lo localmente na mesma pasta onde o setup.exe reside. 
    
    **Observação:** Instalação do Office comumente ocorrer problemas de vencimento para configurado incorretamente ou malformatted arquivos de configuração. Para evitar esses problemas, recomendamos que você use a ferramenta de personalização do Office para criar o arquivo de configuração. Você também pode importar arquivos de configuração existentes para a ferramenta de personalização do Office. 
    
3. Em um prompt de comando elevado, alterne para o local onde residem os setup.exe e executar a ferramenta de implantação do Office no modo download e especifique o arquivo de configuração que você acabou de ser salvo. Neste exemplo, o arquivo de configuração é chamado Configuration. XML:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Executar a ferramenta de implantação do Office no modo de configuração e especifique o arquivo de configuração.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Observação:** Você deve executar esta etapa no computador cliente no qual você deseja instalar o Office e você deve ter permissões de administrador local no computador. 
    
Para saber mais sobre como usar a ferramenta de implantação do Office para os seus cenários de implantação de Office 365 ProPlus, consulte [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Para obter mais detalhes sobre como usar a ferramenta de personalização do Office, consulte [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

