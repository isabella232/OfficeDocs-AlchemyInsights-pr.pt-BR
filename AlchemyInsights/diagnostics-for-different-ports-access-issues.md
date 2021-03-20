---
title: Diagnóstico de diferentes problemas de acesso a portas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897360"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="8aca8-102">Diagnóstico de diferentes problemas de acesso a portas</span><span class="sxs-lookup"><span data-stu-id="8aca8-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="8aca8-103">Para resolver os diferentes problemas de acesso a portas, execute as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="8aca8-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="8aca8-104">Pare/desaloque a máquina virtual (VM) do portal, reinicie a VM e teste novamente.</span><span class="sxs-lookup"><span data-stu-id="8aca8-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="8aca8-105">Verifique as configurações de rede da sua VM para determinar se há NSGs (Grupos de Segurança de Rede) bloqueando o tráfego.</span><span class="sxs-lookup"><span data-stu-id="8aca8-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="8aca8-106">Você também pode usar a [ferramenta de verificação de fluxo IP do Observador de Rede](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) para verificar se NSGs estão bloqueando tráfego, rotas definidas pelo usuário (UDRs) redirecionando o tráfego de volta para o local ('Rota padrão' 0.0.0.0/0) ou para um dispositivo de rede.</span><span class="sxs-lookup"><span data-stu-id="8aca8-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="8aca8-107">Se você ainda tiver problemas depois de tentar as etapas acima, forneça o nome da VM e da porta TCP em que está tentando enviar email para diagnóstico posterior.</span><span class="sxs-lookup"><span data-stu-id="8aca8-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="8aca8-108">**Documentos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="8aca8-108">**Recommended Documents**</span></span>

[<span data-ttu-id="8aca8-109">Limitações e recomendações para o envio de emails de saída pela porta 25</span><span class="sxs-lookup"><span data-stu-id="8aca8-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)