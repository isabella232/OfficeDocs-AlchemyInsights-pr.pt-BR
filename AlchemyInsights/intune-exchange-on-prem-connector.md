---
title: Conector local do Exchange do Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791338"
---
# <a name="intune-exchange-on-premise-connector"></a>Conector local do Exchange do Intune

Para obter detalhes sobre como configurar o conector entre o Intune e o Exchange que estão hospedados no local, consulte a seguinte documentação:

[Configurar o conector do Exchange local do Intune no Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Perguntas Freqüentes:**

P: Eu vejo um erro como "a versão do Exchange Connector não é suportada" ao tentar configurar o Exchange Connector. O que pode ser a causa?

A: a conta que você está usando é licenciada apropriadamente-deve ter uma licença do Active Intune

P: é possível ter vários conectores do Exchange?

A: você só pode configurar um Exchange Connector por locatário do Intune por organização do Exchange. O conector só pode ser instalado em um servidor em uma organização do Exchange de vários servidores.

Além disso, não é possível ter conectores configurados para o Exchange local e o Exchange Online configurados no mesmo locatário.

P: o conector pode usar uma matriz CAS como sua conexão com o Exchange?

A: a especificação de uma matriz CAS não é uma configuração suportada na configuração do conector. Apenas um único servidor deve ser especificado e deve ser codificado no arquivo de configuração do conector, que pode ser encontrado no

Program Data\Microsoft\Microsoft Intune no Exchange Connector local \ OnpremiseExchangeConnectorServiceConfiguration.xml

Localize a seguinte entrada ```<ExchangeWebServiceURL />``` e substitua a URL pelo servidor Exchange.

**Como**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Confira a seguinte documentação para solução de problemas adicional: [solucionar problemas do conector do Exchange local do Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Habilitando o registro detalhado do conector do Exchange**

1. Abra o arquivo de configuração de rastreamento do Exchange Connector para edição.  
O arquivo está localizado em:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Como**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Localize o TraceSourceLine com a seguinte chave: OnPremisesExchangeConnectorService  
  
3. Alterar o valor do nó SourceLevel da informação ActivityTracing (o padrão) para o ActivityTracing detalhado  

**Exemplo:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Reiniciar o serviço do Exchange do Microsoft Intune  
5. Sincronização completa no portal do Intune até que ela seja concluída e, em seguida, altere o XML de volta para "Information ActivityTracing" e reinicie o serviço do Exchange do Microsoft Intune.  
6. O local dos logs é: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`