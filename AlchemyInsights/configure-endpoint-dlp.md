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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657917"
---
# <a name="configure-endpoint-dlp"></a>Configurar o Microsoft Endpoint DLP

O Microsoft Endpoint DLP permite estender a capacidade de proteção e monitoramento de DLP a informações confidenciais em dispositivos com Windows 10. Depois que os dispositivos são integrados ao gerenciamento de dispositivos, você pode criar diretrizes de DLP para impor ações de proteção aos itens. O Gerenciador de Atividade pode ser usado para monitorar a atividade de itens confidenciais. Para mais informações, consulte [Dispositivo Integrados no gerenciamento de dispositivos](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Iniciando com o Endpoint DLP:

- Verifique se você possui o licenciamento apropriado de SKU/assinaturas. Para mais informações, consulte [licenciamento de SKU/assinaturas.](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verifique as permissões exigidas para habilitar o gerenciamento de dispositivos, acessar a página de integração ou ativar/desativar o monitoramento de dispositivos. Para mais informações, confira [Permissões](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Dispositivos integrados no Gerenciamento de dispositivos, seguindo o procedimento de dispositivos integrados. Para mais informações, consulte [Integração de Dispositivo](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Crie diretrizes de DLP para proteger seus itens sigilosos. Para mais informações, consulte [Cenários da diretriz DLP do Endpoint](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Para obter mais informações sobre o Microsoft Endpoint DLP, consulte [Saiba mais sobre a prevenção de perda de dados do Microsoft 365 Endpoint (visualização)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Etapas de coleta de dados importantes, caso o suporte seja necessário:**

1. Baixe o [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Execute a ferramenta como Administrador na janela do cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Quando for solicitado **Insira o número de minutos para coletar rastreamentos:**, insira o número de minutos necessários para executar o cenário.
1. Execute o cenário.

Coletar a saída do arquivo ZIP para entregar ao agente de suporte.
