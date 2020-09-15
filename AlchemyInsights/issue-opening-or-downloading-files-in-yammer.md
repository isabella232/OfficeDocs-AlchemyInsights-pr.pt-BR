---
title: Problema ao abrir ou baixar arquivos no Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695637"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="fdc89-102">Problema ao abrir ou baixar arquivos no Yammer</span><span class="sxs-lookup"><span data-stu-id="fdc89-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="fdc89-103">O Yammer clássico tem suporte para várias opções de carregamentos de arquivos para mensagens e grupos.</span><span class="sxs-lookup"><span data-stu-id="fdc89-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="fdc89-104">Dependendo da configuração de rede, arquivos são armazenados no SharePoint por regra.</span><span class="sxs-lookup"><span data-stu-id="fdc89-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="fdc89-105">O seletor de arquivos no novo Yammer ainda não tem suporte para todas as opções disponíveis no Yammer clássico.</span><span class="sxs-lookup"><span data-stu-id="fdc89-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="fdc89-106">Uma atualização futura adicionará novos recursos.</span><span class="sxs-lookup"><span data-stu-id="fdc89-106">A future update will add additional features.</span></span> <span data-ttu-id="fdc89-107">Para saber mais, confira [Anexar um arquivo ou imagem a uma conversa no Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="fdc89-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="fdc89-108">**Não é possível abrir ou baixar um arquivo**</span><span class="sxs-lookup"><span data-stu-id="fdc89-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="fdc89-109">Um arquivo pode ser carregado no Yammer mas também ser vinculado a um arquivo no SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fdc89-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="fdc89-110">Para solucionar esse problema, primeiro você precisa determinar o local desse arquivo.</span><span class="sxs-lookup"><span data-stu-id="fdc89-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="fdc89-111">Se o arquivo tiver sido carregado no Yammer, ele terá uma URL \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="fdc89-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="fdc89-112">Verifique que os URLs e os endereços de IP necessários estão desbloqueados.</span><span class="sxs-lookup"><span data-stu-id="fdc89-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="fdc89-113">Para saber mais, confira o post do blog[Usando endereços de IP embutidos no Yammer não é recomendável](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="fdc89-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="fdc89-114">Verifique se um usuário que também é um administrador global pode baixar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="fdc89-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="fdc89-115">Se o arquivo for privado, talvez seja necessário usar o modo de conteúdo particular.</span><span class="sxs-lookup"><span data-stu-id="fdc89-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="fdc89-116">Para saber mais, confira [Monitorar conteúdo particular no Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="fdc89-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="fdc89-117">**Convidados no nível da rede do Yammer e arquivos no SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="fdc89-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="fdc89-118">[Os convidados no nível da rede no Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) não usam o Azure AD B2B e são internos do serviço Yammer, portanto, não podem acessar arquivos do Yammer armazenados no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fdc89-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="fdc89-119">Crie um usuário AAD B2B que possa acessar documentos na biblioteca no SharePoint Online usando essa identidade.</span><span class="sxs-lookup"><span data-stu-id="fdc89-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="fdc89-120">Para obter informações sobre o futuro suporte a clientes B2B do Azure AD no Yammer, confira [suporte para Convidados B2B (Business-to-Business) na visualização do Yammer - Termos e perguntas frequentes](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="fdc89-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>