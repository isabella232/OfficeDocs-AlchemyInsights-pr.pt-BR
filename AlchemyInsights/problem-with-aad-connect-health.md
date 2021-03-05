---
title: Problema com a saúde do AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453286"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="86eb5-102">Problema com a saúde do AAD Connect</span><span class="sxs-lookup"><span data-stu-id="86eb5-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="86eb5-103">Certifique-se de que você está autorizado a executar a operação.</span><span class="sxs-lookup"><span data-stu-id="86eb5-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="86eb5-104">Os administradores globais têm acesso por padrão.</span><span class="sxs-lookup"><span data-stu-id="86eb5-104">Global Admins have access by default.</span></span> <span data-ttu-id="86eb5-105">Além disso, você pode usar [o Controle de Acesso Baseado em Função para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar a permissão de registro ao Colaborador.</span><span class="sxs-lookup"><span data-stu-id="86eb5-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="86eb5-106">Verifique se os pontos de extremidade necessários estão habilitados e não bloqueados devido ao firewall.</span><span class="sxs-lookup"><span data-stu-id="86eb5-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="86eb5-107">Para obter detalhes, consulte [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="86eb5-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="86eb5-108">O registro pode falhar devido à comunicação de saída estar sujeita à inspeção SSL pela camada de rede.</span><span class="sxs-lookup"><span data-stu-id="86eb5-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="86eb5-109">Certifique-se de ter verificado as configurações de notificação para o Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="86eb5-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="86eb5-110">Revise sua configuração.</span><span class="sxs-lookup"><span data-stu-id="86eb5-110">Please review your setting.</span></span> <span data-ttu-id="86eb5-111">Este [guia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) pode ajudá-lo a entender como configurar as configurações de notificação para notificações de saúde do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="86eb5-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="86eb5-112">Para saber mais sobre o relatório de sincronização do AAD Connect Health e como baixá-lo, consulte Relatório de [sincronização](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)de nível de objeto .</span><span class="sxs-lookup"><span data-stu-id="86eb5-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="86eb5-113">Para solucionar problemas de alertas de Saúde do AAD Connect, siga o guia de solução de problemas para alertas de atratividade de dados do AAD Connect Health e para perguntas [frequentes,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) consulte [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="86eb5-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
