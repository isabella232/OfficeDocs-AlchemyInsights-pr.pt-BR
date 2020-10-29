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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="1a036-102">Conector local do Exchange do Intune</span><span class="sxs-lookup"><span data-stu-id="1a036-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="1a036-103">Para obter detalhes sobre como configurar o conector entre o Intune e o Exchange que estão hospedados no local, consulte a seguinte documentação:</span><span class="sxs-lookup"><span data-stu-id="1a036-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="1a036-104">Configurar o conector do Exchange local do Intune no Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="1a036-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="1a036-105">**Perguntas Freqüentes:**</span><span class="sxs-lookup"><span data-stu-id="1a036-105">**FAQ:**</span></span>

<span data-ttu-id="1a036-106">P: Eu vejo um erro como "a versão do Exchange Connector não é suportada" ao tentar configurar o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="1a036-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="1a036-107">O que pode ser a causa?</span><span class="sxs-lookup"><span data-stu-id="1a036-107">What could be the cause?</span></span>

<span data-ttu-id="1a036-108">A: a conta que você está usando é licenciada apropriadamente-deve ter uma licença do Active Intune</span><span class="sxs-lookup"><span data-stu-id="1a036-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="1a036-109">P: é possível ter vários conectores do Exchange?</span><span class="sxs-lookup"><span data-stu-id="1a036-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="1a036-110">A: você só pode configurar um Exchange Connector por locatário do Intune por organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a036-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="1a036-111">O conector só pode ser instalado em um servidor em uma organização do Exchange de vários servidores.</span><span class="sxs-lookup"><span data-stu-id="1a036-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="1a036-112">Além disso, não é possível ter conectores configurados para o Exchange local e o Exchange Online configurados no mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="1a036-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="1a036-113">P: o conector pode usar uma matriz CAS como sua conexão com o Exchange?</span><span class="sxs-lookup"><span data-stu-id="1a036-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="1a036-114">A: a especificação de uma matriz CAS não é uma configuração suportada na configuração do conector.</span><span class="sxs-lookup"><span data-stu-id="1a036-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="1a036-115">Apenas um único servidor deve ser especificado e deve ser codificado no arquivo de configuração do conector, que pode ser encontrado no</span><span class="sxs-lookup"><span data-stu-id="1a036-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="1a036-116">Program Data\Microsoft\Microsoft Intune no Exchange Connector local \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="1a036-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="1a036-117">Localize a seguinte entrada ```<ExchangeWebServiceURL />``` e substitua a URL pelo servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a036-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="1a036-118">**Como**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="1a036-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="1a036-119">Confira a seguinte documentação para solução de problemas adicional: [solucionar problemas do conector do Exchange local do Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="1a036-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="1a036-120">**Habilitando o registro detalhado do conector do Exchange**</span><span class="sxs-lookup"><span data-stu-id="1a036-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="1a036-121">Abra o arquivo de configuração de rastreamento do Exchange Connector para edição.</span><span class="sxs-lookup"><span data-stu-id="1a036-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="1a036-122">O arquivo está localizado em:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="1a036-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="1a036-123">**Como**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="1a036-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="1a036-124">Localize o TraceSourceLine com a seguinte chave: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="1a036-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="1a036-125">Alterar o valor do nó SourceLevel da informação ActivityTracing (o padrão) para o ActivityTracing detalhado</span><span class="sxs-lookup"><span data-stu-id="1a036-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="1a036-126">**Exemplo:**</span><span class="sxs-lookup"><span data-stu-id="1a036-126">**Example:**</span></span>
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
4. <span data-ttu-id="1a036-127">Reiniciar o serviço do Exchange do Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1a036-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="1a036-128">Sincronização completa no portal do Intune até que ela seja concluída e, em seguida, altere o XML de volta para "Information ActivityTracing" e reinicie o serviço do Exchange do Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="1a036-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="1a036-129">O local dos logs é: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="1a036-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>