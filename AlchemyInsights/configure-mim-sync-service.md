---
title: Configurar o serviço de Sincronização MIM
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430707"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="0ecea-102">Configurar o serviço de Sincronização MIM</span><span class="sxs-lookup"><span data-stu-id="0ecea-102">Configure MIM Sync service</span></span>

<span data-ttu-id="0ecea-103">O Serviço de Sincronização Microsoft Identity Manager (MIM) é um componente do MIM.</span><span class="sxs-lookup"><span data-stu-id="0ecea-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="0ecea-104">É um serviço local centralizado que armazena e integra informações para organizações que possuem vários diretórios e bancos de dados locais.</span><span class="sxs-lookup"><span data-stu-id="0ecea-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="0ecea-105">Você pode resolver o seu problema com a Sincronização MIM se o problema foi abordado em uma atualização recente do MIM ou se for um dos outros problemas mencionados na seção abaixo.</span><span class="sxs-lookup"><span data-stu-id="0ecea-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="0ecea-106">**Etapas recomendadas**</span><span class="sxs-lookup"><span data-stu-id="0ecea-106">**Recommended steps**</span></span>

1. <span data-ttu-id="0ecea-107">Certifique-se de estar usando uma atualização recente da Sincronização MIM e verifique as [observações de versão da Sincronizar MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) para determinar se o problema foi resolvido em uma atualização.</span><span class="sxs-lookup"><span data-stu-id="0ecea-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="0ecea-108">Se o problema for com o conector LDAP Genérico, SQL Genérico, Lotus Domino ou conector de Serviços Web, certifique-se de estar usando uma atualização recente dos [conectores genéricos](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="0ecea-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="0ecea-109">Se a execução de uma Sincronização MIM parar com um erro, consulte a tabela de [códigos de erro de execução](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) para determinar as causas potenciais.</span><span class="sxs-lookup"><span data-stu-id="0ecea-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="0ecea-110">Se a execução for interrompida com a **exceção de extensão dll**, clique nessas palavras para abrir a janela **Propriedades do Objeto do Espaço Conector** e clique em **Rastreamento de Pilha...** para consultar mais informações sobre a causa subjacente, conforme descrito na [Exceção de Extensão DLL](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="0ecea-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="0ecea-111">Se o componente Serviço de Notificação de alteração de Senha (PCNS) relatar o **erro 6025** no log de eventos durante a sincronização de senha, verifique o guia de solução de problemas [PCNS relatando o erro 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="0ecea-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="0ecea-112">Se a sincronização completa com o Agente de Gerenciamento de Serviço FIM for lenta, verifique a configuração de **crescimento automático** para TempDB, conforme descrito em [Solução de problemas de sincronização lenta ou total suspensa](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="0ecea-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="0ecea-113">Se você estiver encontrando um erro de servidor parado com falha na criação por meio de serviços web usando o Agente de Gerenciamento de Serviços FIM, consulte [Informações de Suporte: falha na criação por meio de serviços web](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) para uma visão geral das causas.</span><span class="sxs-lookup"><span data-stu-id="0ecea-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

