---
title: Criando políticas de rótulo do AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542068"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="fde8b-102">Criando políticas de rótulo do AIP</span><span class="sxs-lookup"><span data-stu-id="fde8b-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="fde8b-103">Os rótulos da proteção de informações do Azure (AIP) podem ser usados com o intervalo completo de dados que uma organização normalmente cria e armazena, da classificação mais baixa de dados pessoais, à classificação mais alta de dados altamente confidenciais.</span><span class="sxs-lookup"><span data-stu-id="fde8b-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="fde8b-104">As políticas de proteção de informações do Azure se aplicam ao cliente clássico da proteção de informações do Azure (AIP) e não ao [cliente de rotulação unificado do AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="fde8b-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="fde8b-105">Você pode configurar vários elementos em uma política de AIP, incluindo opções como:</span><span class="sxs-lookup"><span data-stu-id="fde8b-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="fde8b-106">Opção para qual rótulo permitirá que administradores ou usuários classifiquem e (opcionais) documentos e emails</span><span class="sxs-lookup"><span data-stu-id="fde8b-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="fde8b-107">Opção para impor a classificação quando os usuários salvam documentos e enviam emails</span><span class="sxs-lookup"><span data-stu-id="fde8b-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="fde8b-108">Opção para rotular automaticamente uma mensagem de email com base em seus anexos.</span><span class="sxs-lookup"><span data-stu-id="fde8b-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="fde8b-109">Opção para controlar se a barra de proteção de informações é exibida em aplicativos do Office</span><span class="sxs-lookup"><span data-stu-id="fde8b-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="fde8b-110">Para obter mais opções e informações sobre as políticas de proteção de informações do Azure, consulte: [visão geral da política de proteção de informações do Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="fde8b-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="fde8b-111">Para outros recursos úteis referentes a políticas do AIP, consulte:</span><span class="sxs-lookup"><span data-stu-id="fde8b-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="fde8b-112">Tutorial: definir as configurações da política de proteção de informações do Azure e criar um novo rótulo</span><span class="sxs-lookup"><span data-stu-id="fde8b-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="fde8b-113">Configurando a política de proteção de informações do Azure</span><span class="sxs-lookup"><span data-stu-id="fde8b-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="fde8b-114">Criar e configurar rótulos de confidencialidade e suas políticas</span><span class="sxs-lookup"><span data-stu-id="fde8b-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="fde8b-115">Guias de instruções para cenários comuns que usam a proteção de informações do Azure</span><span class="sxs-lookup"><span data-stu-id="fde8b-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="fde8b-116">Analisar a documentação de proteção de informações do Azure</span><span class="sxs-lookup"><span data-stu-id="fde8b-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="fde8b-117">Requisitos para a proteção de informações do Azure</span><span class="sxs-lookup"><span data-stu-id="fde8b-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="fde8b-118">Tutorial de início rápido para a proteção de informações do Azure</span><span class="sxs-lookup"><span data-stu-id="fde8b-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="fde8b-119">Baixar o cliente de proteção de informações do Azure</span><span class="sxs-lookup"><span data-stu-id="fde8b-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)