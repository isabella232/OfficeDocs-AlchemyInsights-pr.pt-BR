---
title: Criando políticas de rótulo do AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732163"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="7980a-102">Criando políticas de rótulo do AIP</span><span class="sxs-lookup"><span data-stu-id="7980a-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="7980a-103">Os rótulos da proteção de informações do Azure (AIP) podem ser usados com o intervalo completo de dados que uma organização normalmente cria e armazena, da classificação mais baixa de dados pessoais, à classificação mais alta de dados altamente confidenciais.</span><span class="sxs-lookup"><span data-stu-id="7980a-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="7980a-104">As políticas de proteção de informações do Azure se aplicam ao cliente clássico da proteção de informações do Azure (AIP) e não ao  [cliente de rotulação unificado do AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="7980a-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="7980a-105">Você pode configurar vários elementos em uma política de AIP, incluindo opções como:</span><span class="sxs-lookup"><span data-stu-id="7980a-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="7980a-106">Opção para qual rótulo permitirá que administradores ou usuários classifiquem e (opcionais) documentos e emails</span><span class="sxs-lookup"><span data-stu-id="7980a-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="7980a-107">Opção para impor a classificação quando os usuários salvam documentos e enviam emails</span><span class="sxs-lookup"><span data-stu-id="7980a-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="7980a-108">Opção para rotular automaticamente uma mensagem de email com base em seus anexos.</span><span class="sxs-lookup"><span data-stu-id="7980a-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="7980a-109">Opção para controlar se a barra de proteção de informações é exibida em aplicativos do Office</span><span class="sxs-lookup"><span data-stu-id="7980a-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="7980a-110">Para obter mais opções e informações sobre as políticas de proteção de informações do Azure, consulte: [visão geral da política de proteção de informações do Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="7980a-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="7980a-111">Para outros recursos úteis referentes a políticas do AIP, consulte:</span><span class="sxs-lookup"><span data-stu-id="7980a-111">For other helpful resources regarding AIP policies, see:</span></span>

- <span data-ttu-id="7980a-112">[Tutorial: Configure as configurações da política do Serviço de Proteção de Informações do Azure e crie um novo rótulo](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="7980a-112">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)</span></span>  
- [<span data-ttu-id="7980a-113">Configurando a política do Serviço de Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="7980a-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="7980a-114">Criar e configurar rótulos de confidencialidade e suas políticas</span><span class="sxs-lookup"><span data-stu-id="7980a-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="7980a-115">Guias de instruções para cenários comuns que usam a Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="7980a-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="7980a-116">Analisar a documentação da Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="7980a-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- <span data-ttu-id="7980a-117">[Requisitos da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="7980a-117">[Requirements for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span></span>  
- <span data-ttu-id="7980a-118">[Tutorial de início rápido da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="7980a-118">[Quick start tutorial for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)</span></span>  
- [<span data-ttu-id="7980a-119">Baixar o cliente da Proteção de Informações do Azure</span><span class="sxs-lookup"><span data-stu-id="7980a-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)