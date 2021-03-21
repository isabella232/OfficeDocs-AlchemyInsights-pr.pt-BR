---
title: Importar e Exportar do Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897404"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="f0c39-102">Importar e Exportar do Yammer</span><span class="sxs-lookup"><span data-stu-id="f0c39-102">Import and export from Yammer</span></span>

<span data-ttu-id="f0c39-103">**Importação**</span><span class="sxs-lookup"><span data-stu-id="f0c39-103">**Import**</span></span>

<span data-ttu-id="f0c39-104">As opções de importação do usuário variam dependendo se a sua rede do Yammer está ou não no [Modo Nativo para Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode).</span><span class="sxs-lookup"><span data-stu-id="f0c39-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="f0c39-105">**Modo não nativo**: os usuários podem ser importados para grupos usando o [Adicionar do Catálogo de Endereços](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limite de 100 usuários) nas configurações do grupo ou para a rede usando o [Atualização em Massa](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) no Administrador de Rede.</span><span class="sxs-lookup"><span data-stu-id="f0c39-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="f0c39-106">**Modo Nativo**: as operações de associação a um grupo e de associação de rede devem ser executadas no [Portal de administração do Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [Portal do Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ou usando outra opção do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0c39-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="f0c39-107">As redes no Modo Nativo não têm mais acesso à Atualização em Massa e a outros recursos herdados.</span><span class="sxs-lookup"><span data-stu-id="f0c39-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f0c39-108">O Yammer nunca teve suporte para a importação de conteúdo dentro do Administrador de Rede mesmo quando o recurso Exportação de Dados era usado em outra rede.</span><span class="sxs-lookup"><span data-stu-id="f0c39-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="f0c39-109">O conteúdo pode ser repostado por soluções de parceiros ou pelas APIs REST do Yammer.</span><span class="sxs-lookup"><span data-stu-id="f0c39-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="f0c39-110">**Exportar**</span><span class="sxs-lookup"><span data-stu-id="f0c39-110">**Export**</span></span>

<span data-ttu-id="f0c39-111">[Exportar Dados de Rede dentro do Administrador de Rede](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permite a exportação de conteúdo de redes do Yammer, incluindo mensagens e arquivos.</span><span class="sxs-lookup"><span data-stu-id="f0c39-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="f0c39-112">Os anexos podem ser extremamente grandes e farão com que as exportações demorem muito para serem concluídas.</span><span class="sxs-lookup"><span data-stu-id="f0c39-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="f0c39-113">Recomendamos que as redes ativas sejam exportadas usando a [API de Exportação de Dados](https://developer.yammer.com/docs/data-export-api) em blocos por dia ou por semana.</span><span class="sxs-lookup"><span data-stu-id="f0c39-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="f0c39-114">O Suporte da Microsoft não fornece scripts personalizados para essa finalidade.</span><span class="sxs-lookup"><span data-stu-id="f0c39-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="f0c39-115">Uma [Exportação de GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) separada existe para exportar o conteúdo para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="f0c39-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>