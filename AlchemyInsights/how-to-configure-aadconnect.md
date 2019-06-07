---
title: 646 como configurar o AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 2dc4ae7d6809c24ce599ac128570e9354c9f2b30
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752549"
---
# <a name="configure-sync-features"></a><span data-ttu-id="50638-102">Configurar recursos de sincronização</span><span class="sxs-lookup"><span data-stu-id="50638-102">Configure sync features</span></span>

<span data-ttu-id="50638-103">O Azure AD Connect inclui vários recursos habilitados por padrão ou que você pode habilitar posteriormente.</span><span class="sxs-lookup"><span data-stu-id="50638-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="50638-104">Alguns recursos exigem configuração adicional em ambientes específicos.</span><span class="sxs-lookup"><span data-stu-id="50638-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="50638-105">[Filtrando](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limites os objetos estão sincronizados com o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50638-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="50638-106">Por padrão, todos os usuários, contatos, grupos e contas de computador do Windows 10 são sincronizados.</span><span class="sxs-lookup"><span data-stu-id="50638-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="50638-107">Você pode incluir ou excluir objetos com base em domínios, UOs ou outros atributos.</span><span class="sxs-lookup"><span data-stu-id="50638-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="50638-108">A [sincronização de hash de senha](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de senha do Active Directory local para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50638-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="50638-109">Isso permite o gerenciamento de senhas em um local, mas o uso da mesma senha em ambientes locais e em nuvem.</span><span class="sxs-lookup"><span data-stu-id="50638-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="50638-110">Como o Active Directory é a fonte autoritativa, você pode usar suas próprias diretivas de senha.</span><span class="sxs-lookup"><span data-stu-id="50638-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="50638-111">[A redefinição de senha de autoatendimento (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que os usuários redefinam suas próprias senhas na nuvem enquanto ainda aplicam sua política de senha local.</span><span class="sxs-lookup"><span data-stu-id="50638-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="50638-112">O [write-back de dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que dispositivos registrados no Azure ad sejam gravados novamente no Active Directory local para que possam ser usados para acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="50638-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="50638-113">[Impedir que exclusões acidentais](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) sejam habilitadas por padrão para ajudar a evitar muitas exclusões de objetos simultâneas (mais de 500 objetos por sincronização).</span><span class="sxs-lookup"><span data-stu-id="50638-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="50638-114">Você pode alterar essa configuração para atender às necessidades da sua organização.</span><span class="sxs-lookup"><span data-stu-id="50638-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="50638-115">A [atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está habilitada por padrão para instalações expressas e ajuda a garantir que sua versão do Azure ad Connect seja sempre atual.</span><span class="sxs-lookup"><span data-stu-id="50638-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
