---
title: O Workday para o Provisionamento de Usuário do AD entra em estado de quarentena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430708"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="67cf3-102">O Workday para o Provisionamento de Usuário do AD entra em estado de quarentena</span><span class="sxs-lookup"><span data-stu-id="67cf3-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="67cf3-103">**O Workday para o Provisionamento de Usuário do AD entra em estado de quarentena e nenhum usuário é criado no AD**</span><span class="sxs-lookup"><span data-stu-id="67cf3-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="67cf3-104">O Workday para o trabalho do Provisionamento de Usuário do AD foi para o estado de quarentena e os logs de auditoria mostram os eventos de falha de exportação com a mensagem de erro **Error: OperationsError-SvcErr: Ocorreu um erro de operação. Nenhuma referência superior foi configurada para o serviço de diretório. O serviço de diretório, portanto, não pode emitir referências a objetos fora desta floresta**.</span><span class="sxs-lookup"><span data-stu-id="67cf3-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="67cf3-105">Esse erro normalmente aparece se o UO do Contêiner do Active Directory não estiver configurado corretamente ou se houver problemas com o Expression Mapping usado para **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="67cf3-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="67cf3-106">Verifique se há erros de digitação no parâmetro UO Padrão para **Novos Usuários**.</span><span class="sxs-lookup"><span data-stu-id="67cf3-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="67cf3-107">Verifique se o UO especificado já existe no seu AD.</span><span class="sxs-lookup"><span data-stu-id="67cf3-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="67cf3-108">Se você estiver usando **parentDistinguishedName** no mapeamento de atributos, verifique se ele sempre avalia para um recipiente conhecido dentro do domínio do AD.</span><span class="sxs-lookup"><span data-stu-id="67cf3-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="67cf3-109">Verifique o evento Exportar nos logs de auditoria para ver o valor gerado.</span><span class="sxs-lookup"><span data-stu-id="67cf3-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="67cf3-110">Para obter mais detalhes sobre como configurar o Workday para provisionamento automatizado, confira [Tutorial: Configurar o Workday para provisionamento automático](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="67cf3-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

