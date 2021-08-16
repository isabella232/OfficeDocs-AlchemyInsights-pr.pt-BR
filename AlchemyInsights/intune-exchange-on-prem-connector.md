---
title: O Intune Exchange conector local
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013952"
---
# <a name="intune-exchange-on-premise-connector"></a>O Intune Exchange conector local

Para obter detalhes sobre como configurar o conector entre o Intune e Exchange que está hospedado no local, consulte a seguinte documentação:

[Configurar o conector de Exchange local do Intune no Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Perguntas Freqüentes:**

P: Eu vejo um erro como "A versão do conector Exchange não é suportada" ao tentar configurar o conector Exchange. Qual pode ser a causa?

R: A conta que você está usando está licenciada adequadamente - ela deve ter uma licença ativa do Intune

P: É possível ter vários Exchange conectores?

R: Você só pode configurar um conector Exchange por locatário do Intune por Exchange organização. O conector só pode ser instalado em um servidor em uma organização de exchange de vários servidores.

Além disso, você não pode ter conectores configurados para o Exchange local e Exchange Online configurados no mesmo locatário.

P: O conector pode usar uma matriz CAS como sua conexão com Exchange?

R: Especificar uma matriz CAS não é uma configuração suportada na configuração do conector. Somente um único servidor deve ser especificado e deve ser hardcoded no arquivo de configuração do conector que pode ser encontrado em

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Localize a entrada a ```<ExchangeWebServiceURL />``` seguir e substitua a URL pelo servidor exchange.

**Exemplo:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Consulte a documentação a seguir para solucionar problemas adicionais: Solucionar problemas do conector de Exchange [local do Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Habilitando o log detalhado para o Exchange conector**

1. Abra o arquivo Exchange configuração de rastreamento do Conector para edição.  
O arquivo está localizado em : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Exemplo:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Localize TraceSourceLine com a seguinte chave: OnPremisesExchangeConnectorService  
  
3. Alterar o valor do nó SourceLevel de Information ActivityTracing (o padrão) para Verbose ActivityTracing  

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
4. Reiniciar o serviço Microsoft Intune Exchange de usuário  
5. Sincronização completa no Portal do Intune até que ele termine e altere o XML de volta para "Information ActivityTracing" e reinicie o serviço Microsoft Intune Exchange.  
6. O local dos logs é : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`