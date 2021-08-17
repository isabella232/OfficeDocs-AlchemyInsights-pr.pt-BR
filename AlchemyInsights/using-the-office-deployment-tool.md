---
title: Usando a ferramenta Office implantação
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083758"
---
# <a name="using-the-office-deployment-tool-odt"></a>Usando a Office de Implantação (ODT)

Você usa a Office de Implantação (ODT) para implantar Office 365 versões do Office. A Office de Implantação (setup.exe) é executado a partir da linha de comando e usa um arquivo XML de configuração para determinar quais configurações serão aplicadas ao implantar Office.
  
1. Baixe a versão mais recente da ferramenta Office de Implantação do [Centro de Download da Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Use a Office ferramenta de [personalização (OCT)](https://config.office.com) para selecionar suas preferências de implantação e criar o arquivo XML de configuração. Exporte o arquivo de configuração e coloque-o localmente na mesma pasta onde o setup.exe reside.

    **Observação: Office** de instalação geralmente ocorrem devido a arquivos de configuração mal configurados ou malformados. Para evitar esses problemas, recomendamos que você use Office Ferramenta de Personalização para criar o arquivo de configuração. Você também pode importar arquivos de configuração existentes para a ferramenta Office Personalização.

3. Em um prompt de comando elevado, alterna para o local onde setup.exe reside e execute a Ferramenta de Implantação Office no modo de download e especifique o arquivo de configuração que você acabou de salvar. Neste exemplo, o arquivo de configuração é chamado Configuration.xml:

```setup.exe /download Configuration.xml```

4.Execute o Office de Implantação no modo de configuração e especifique o arquivo de configuração.

```setup.exe /configure Configuration.xml```

**Observação:** Você deve executar esta etapa do computador cliente no qual deseja instalar Office e você deve ter permissões de administrador local nesse computador.

Para saber mais sobre como usar Office Ferramenta de Implantação para seus Microsoft 365 Apps para Grandes Empresas de implantação, consulte [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Para obter mais detalhes sobre como usar a ferramenta de personalização Office, consulte [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
