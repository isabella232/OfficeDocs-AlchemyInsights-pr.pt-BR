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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030890"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnóstico de diferentes problemas de acesso a portas

Para resolver os diferentes problemas de acesso a portas, execute as seguintes etapas:

1. Pare/desaloque a máquina virtual (VM) do portal, reinicie a VM e teste novamente. 
2. Verifique as configurações de rede da sua VM para determinar se há NSGs (Grupos de Segurança de Rede) bloqueando o tráfego. Você também pode usar a [ferramenta de verificação de fluxo IP do Observador de Rede](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) para verificar se NSGs estão bloqueando tráfego, rotas definidas pelo usuário (UDRs) redirecionando o tráfego de volta para o local ('Rota padrão' 0.0.0.0/0) ou para um dispositivo de rede.
Se você ainda tiver problemas depois de tentar as etapas acima, forneça o nome da VM e da porta TCP em que está tentando enviar email para diagnóstico posterior.

**Documentos Recomendados**

[Limitações e recomendações para o envio de emails de saída pela porta 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)