---
title: Usando a ferramenta de implantação do Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085820"
---
# <a name="using-the-office-deployment-tool-odt"></a>Usando a ferramenta de implantação do Office (ODT)

Use a ferramenta de implantação do Office (ODT) para implantar versões do Office 365. A ferramenta de implantação do Office (setupodt.exe) é executada a partir da linha de comando e usa um arquivo XML de configuração para determinar quais configurações serão aplicadas durante a implantação do Office.
  
1. Baixe a versão mais recente da ferramenta de implantação do Office no [centro de download da Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Use a [ferramenta de personalização do Office (OCT)](https://config.office.com) para selecionar suas preferências de implantação e criar o arquivo XML de configuração. Exporte o arquivo de configuração e coloque-o localmente na mesma pasta onde o setupodt.exe reside.

    **Observação:** Problemas de instalação do Office geralmente ocorrem devido a arquivos de configuração incorretamente configurados ou malformatted. Para evitar esses problemas, recomendamos que você use a ferramenta de personalização do Office para criar o arquivo de configuração. Você também pode importar arquivos de configuração existentes para a ferramenta de personalização do Office.

3. Em um prompt de comando com privilégios elevados, alterne para o local onde setupodt.exe residem e execute a ferramenta de implantação do Office no modo de download e especifique o arquivo de configuração que você acabou de salvar. Neste exemplo, o arquivo de configuração é chamado Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Execute a ferramenta de implantação do Office no modo de configuração e especifique o arquivo de configuração.

```setupodt.exe /configure Configuration.xml```

**Observação:** Você deve executar esta etapa no computador cliente no qual você deseja instalar o Office e deve ter permissões de administrador local nesse computador.

Para saber mais sobre como usar a ferramenta de implantação do Office para seus aplicativos do Microsoft 365 para cenários de implantação corporativa, confira [visão geral da ferramenta de implantação do Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Para obter mais detalhes sobre como usar a ferramenta de personalização do Office, consulte [visão geral da ferramenta de personalização do Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
