---
title: Usando a ferramenta de implantação do Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365513"
---
# <a name="using-the-office-deployment-tool-odt"></a>Usando a ferramenta de implantação do Office (ODT)

Use a ferramenta de implantação do Office (ODT) para implantar versões do Office 365. A ferramenta de implantação do Office (Setup. exe) é executada a partir da linha de comando e usa um arquivo XML de configuração para determinar quais configurações serão aplicadas durante a implantação do Office.
  
1. Baixe a versão mais recente da ferramenta de implantação do Office no [centro de download da Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Use a [ferramenta de personalização do Office (OCT)](https://config.office.com) para selecionar suas preferências de implantação e criar o arquivo XML de configuração. Exporte o arquivo de configuração e coloque-o localmente na mesma pasta em que reside o setup. exe.

    **Observação:** Problemas de instalação do Office geralmente ocorrem devido a arquivos de configuração incorretamente configurados ou malformatted. Para evitar esses problemas, recomendamos que você use a ferramenta de personalização do Office para criar o arquivo de configuração. Você também pode importar arquivos de configuração existentes para a ferramenta de personalização do Office.

3. Em um prompt de comando com privilégios elevados, alterne para o local em que o setup. exe reside e execute a ferramenta de implantação do Office no modo de download e especifique o arquivo de configuração que você acabou de salvar. Neste exemplo, o arquivo de configuração é chamado de Configuration. xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Execute a ferramenta de implantação do Office no modo de configuração e especifique o arquivo de configuração.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Observação:** Você deve executar esta etapa no computador cliente no qual você deseja instalar o Office e deve ter permissões de administrador local nesse computador.

Para saber mais sobre como usar a ferramenta de implantação do Office para seus cenários de implantação do Office 365 ProPlus, confira [visão geral da ferramenta de implantação do Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Para obter mais detalhes sobre como usar a ferramenta de personalização do Office, consulte [visão geral da ferramenta de personalização do Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
