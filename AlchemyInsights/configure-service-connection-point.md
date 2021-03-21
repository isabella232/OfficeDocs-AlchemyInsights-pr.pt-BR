---
title: Configurar ponto de conexão de serviço (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897407"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="6a5b5-102">Configurar ponto de conexão de serviço (SCP)</span><span class="sxs-lookup"><span data-stu-id="6a5b5-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="6a5b5-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="6a5b5-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="6a5b5-104">**Motivo**: não é possível ler o objeto SCP e obter as informações do locatário do Azure AD</span><span class="sxs-lookup"><span data-stu-id="6a5b5-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="6a5b5-105">**Resolução**: confira a seção [Configurar um ponto de conexão de serviço](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="6a5b5-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="6a5b5-106">**Plano de ação**</span><span class="sxs-lookup"><span data-stu-id="6a5b5-106">**Action plan**</span></span>

- <span data-ttu-id="6a5b5-107">Verifique se o dispositivo recebeu o GPO para a validação controlada.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="6a5b5-108">Verifique se o GPO criou as chaves do Registro.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="6a5b5-109">Certifique-se de ter 2 chaves criadas com seu ID de diretório e domínio onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="6a5b5-110">**Definir a configuração do Registro do lado do cliente para SCP**</span><span class="sxs-lookup"><span data-stu-id="6a5b5-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="6a5b5-111">Use o exemplo a seguir para criar um objeto de política de grupo (GPO) para implantar uma configuração de Registro que configure uma entrada SCP no Registro de seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="6a5b5-112">Abra um console de gerenciamento de política de grupo e crie um novo GPO em seu domínio.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="6a5b5-113">Forneça um nome para o GPO recém-criado (por exemplo, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="6a5b5-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="6a5b5-114">Edite o GPO e localize o seguinte caminho: **Configuração do computador > Preferências > Configurações do Windows > Registro**.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="6a5b5-115">Clique com o botão direito em **Registro** e selecione **Novo > Item do Registro**.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="6a5b5-116">Na guia **Geral**, configure o seguinte:</span><span class="sxs-lookup"><span data-stu-id="6a5b5-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="6a5b5-117">**Ação**: atualizar</span><span class="sxs-lookup"><span data-stu-id="6a5b5-117">**Action**: Update</span></span>
    
- <span data-ttu-id="6a5b5-118">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="6a5b5-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="6a5b5-119">**Caminho da chave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="6a5b5-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="6a5b5-120">**Nome do valor**: TenantId</span><span class="sxs-lookup"><span data-stu-id="6a5b5-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="6a5b5-121">**Tipo do valor**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="6a5b5-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="6a5b5-122">**Dados do valor**: o GUID ou ID de diretório da instância do Azure AD (esse valor pode ser encontrado no **portal do Azure > Azure Active Directory > Propriedades > ID de diretório**)</span><span class="sxs-lookup"><span data-stu-id="6a5b5-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="6a5b5-123">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="6a5b5-124">Clique com o botão direito em **Registro** e selecione **Novo > Item do Registro**.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="6a5b5-125">Na guia **Geral**, configure o seguinte:</span><span class="sxs-lookup"><span data-stu-id="6a5b5-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="6a5b5-126">**Ação**: atualizar</span><span class="sxs-lookup"><span data-stu-id="6a5b5-126">**Action**: Update</span></span>
    
- <span data-ttu-id="6a5b5-127">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="6a5b5-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="6a5b5-128">**Caminho da chave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="6a5b5-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="6a5b5-129">**Nome do valor**: TenantName</span><span class="sxs-lookup"><span data-stu-id="6a5b5-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="6a5b5-130">**Tipo do valor**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="6a5b5-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="6a5b5-131">**Dados do valor**: o nome de domínio verificado se você estiver usando um ambiente federado, como AD FS.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="6a5b5-132">O nome de domínio verificado ou o nome de domínio onmicrosoft.com (por exemplo, contoso.onmicrosoft).com se você estiver usando um ambiente gerenciado</span><span class="sxs-lookup"><span data-stu-id="6a5b5-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="6a5b5-133">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-133">Click **OK**.</span></span>

7. <span data-ttu-id="6a5b5-134">Feche o editor do GPO recém-criado.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="6a5b5-135">Vincule o GPO recém-criado à UO desejada contendo computadores associados ao domínio que pertencem ao seu conjunto de dados de distribuição controlado.</span><span class="sxs-lookup"><span data-stu-id="6a5b5-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="6a5b5-136">Para obter mais informações, confira [Validação controlada de associação híbrida do Azure AD - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) e [Solução de problemas de dispositivos híbridos associados ao Azure Active Directory | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="6a5b5-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









