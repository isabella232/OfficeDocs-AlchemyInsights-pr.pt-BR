---
title: Configurar serviço de domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884553"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="45eb4-102">Não é possível habilitar o AAD-DS ou a implantação está falhando</span><span class="sxs-lookup"><span data-stu-id="45eb4-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="45eb4-103">Para resolver o problema que faz com que o serviço de domínio do Azure AD (AAD-DS) não possa ser habilitado ou implantado, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="45eb4-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="45eb4-104">Se você estiver usando uma rede virtual já existente, verifique em seu NSG as regras que bloqueiam as portas necessárias para sincronizar o AAD-DS ao portal https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="45eb4-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="45eb4-105">Verifique se a mensagem de erro foi respondida neste guia de solução de problemas que está disponível em https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="45eb4-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="45eb4-106">Tente implantar o Azure AD Domain Services em uma nova rede virtual.</span><span class="sxs-lookup"><span data-stu-id="45eb4-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="45eb4-107">Siga o guia de Introdução sobre como implantar o AAD-DS: [Criar e configurar o Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="45eb4-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="45eb4-108">Se estiver tendo problemas com a implantação do Azure AD Domain Services, confira [Solucionar Problemas do Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) para resolver erros comuns e ajudá-lo a fazer as coisas funcionarem novamente.</span><span class="sxs-lookup"><span data-stu-id="45eb4-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="45eb4-109">**Não é possível desabilitar o AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="45eb4-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="45eb4-110">O AAD-DS não pode ser pausado.</span><span class="sxs-lookup"><span data-stu-id="45eb4-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="45eb4-111">Se deseja parar de usar seu domínio gerenciado, ele deve ser excluído.</span><span class="sxs-lookup"><span data-stu-id="45eb4-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="45eb4-112">Para excluir seu domínio gerenciado, confira [Excluir serviço de domínio do Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="45eb4-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



