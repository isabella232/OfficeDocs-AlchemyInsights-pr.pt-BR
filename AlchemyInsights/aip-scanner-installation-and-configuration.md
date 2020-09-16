---
title: 'Scanner do AIP: instalação e configuração'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686630"
---
# <a name="aip-scanner-installation-and-configuration"></a>Scanner do AIP: instalação e configuração

**Para instalar o scanner do AIP, siga as diretrizes recomendadas**:

1. Se você estiver atualizando e não iniciando uma instalação do zero, certifique-se de que você seguiu as diretrizes para [atualizando o scanner de Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) e o cliente de rotulagem unificada, confira [atualizando o scanner de Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Verifique se você está em conformidade com todas as [Configurações de firewalls e de infraestrutura de rede](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Verifique se as suas [políticas estão definidas](https://docs.microsoft.com/azure/information-protection/configure-policy) para rotular automaticamente ou tem um rótulo padrão na política.
4. Verifique se o tipo de arquivo relevante está configurado para rótulo/proteção conforme descrito em [Tipos de arquivo suportados pelo cliente de Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Além disso, se você quiser alterar o comportamento padrão, siga estas diretrizes: [Alterar o nível de proteção padrão dos arquivos](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Verifique se a conta de usuário configurada para executar o serviço de scanner têm permissões para acessar todos os repositórios configurados.
6. Se você ainda tiver problemas, exporte os logs do scanner e adicione-os ao seu tíquete de suporte.

**Exportar os logs do Scanner da Proteção de Informações do Azure**

1. Navegue até %localappdata%\Microsoft\MSIP no contexto de usuário que executa o serviço de scanner.
2. Zipar todo o conteúdo na pasta MSIP.
3. Salve os logs no local desejado e anexe-os à sua solicitação de serviço.
4. Você também pode usar [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Confira mais informações em**:
- [Implantação do scanner da Proteção de Informações do Azure para classificar e proteger arquivos automaticamente](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Especificar e usar o Parâmetro de token para Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Executar um ciclo de descoberta e exibir relatórios do scanner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Analisar a documentação da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Requisitos da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Baixar o cliente da Proteção de Informações do Azure](https://www.microsoft.com/download/details.aspx?id=53018)
