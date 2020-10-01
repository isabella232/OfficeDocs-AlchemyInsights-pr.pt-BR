---
title: Configurar o Microsoft Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: d0363d6bdecdb266a5f4a3a14bd496ede6bb9931
ms.sourcegitcommit: 76b147af688f0dc39878a913a050c0e56af054a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2020
ms.locfileid: "48305431"
---
# <a name="configure-endpoint-dlp"></a>Configurar o Microsoft Endpoint DLP

O Microsoft Endpoint DLP permite estender a capacidade de proteção e monitoramento de DLP a informações confidenciais em dispositivos com Windows 10. Depois que os dispositivos são integrados ao gerenciamento de dispositivos, você pode criar diretrizes de DLP para impor ações de proteção aos itens. O Gerenciador de Atividade pode ser usado para monitorar a atividade de itens confidenciais. Para mais informações, consulte [Dispositivo Integrados no gerenciamento de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Iniciando com o Endpoint DLP:

- Verifique se você possui o licenciamento apropriado de SKU/assinaturas. Para mais informações, consulte [licenciamento de SKU/assinaturas.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verifique as permissões exigidas para habilitar o gerenciamento de dispositivos, acessar a página de integração ou ativar/desativar o monitoramento de dispositivos. Para mais informações, consulte [Permissões](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Dispositivos integrados dentro do gerenciamento de dispositivos, seguindo o procedimento de dispositivos integrados. Se você não tiver a opção de Integração de Dispositivo (visualização) em Conformidade com o M365  **Configurações **, confirme se possui a licença e as permissões apropriadas mencionadas acima. Para mais informações, consulte [Integração de Dispositivo](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Crie diretrizes de DLP para proteger seus itens sigilosos. Para mais informações, consulte [Cenários da diretriz DLP do Endpoint](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Para obter mais informações sobre o Microsoft Endpoint DLP, consulte [Saiba mais sobre a prevenção de perda de dados do Microsoft 365 Endpoint (visualização)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Etapas de coleta de dados importantes, caso o suporte seja necessário:**

1. Baixe o MDATP Client Analyzer Preview do [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")
2. Execute a ferramenta como Administrador na janela do cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Quando solicitado "Digite o número de minutos para coletar rastreamentos:", insira o número de minutos necessários para executar o cenário
5. Nome do cenário

Colete a saída do arquivo zip a ser fornecido ao agente de suporte.
