---
title: 646 como configurar AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499658"
---
# <a name="configure-sync-features"></a><span data-ttu-id="71726-102">Configurar recursos de sincronização</span><span class="sxs-lookup"><span data-stu-id="71726-102">Configure sync features</span></span>

<span data-ttu-id="71726-p101">Conectar do Azure AD inclui vários recursos que estão habilitados por padrão, ou que você pode habilitar posteriormente. Alguns recursos exigem configuração adicional em ambientes específicos.</span><span class="sxs-lookup"><span data-stu-id="71726-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="71726-p102">Limites de [filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) os objetos são sincronizados para o Windows Azure AD. Por padrão, todos os usuários, contatos, grupos e Windows 10 contas de computador são sincronizadas. Você pode incluir ou excluir objetos com base em domínios, OUs ou outros atributos.</span><span class="sxs-lookup"><span data-stu-id="71726-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="71726-p103">[Sincronização de hash de senha](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash da senha do Active Directory local para o Windows Azure AD. Isso permite que o gerenciamento de senha em um único local, mas o uso da mesma senha nos dois locais e ambientes em nuvem. Como o Active Directory é a origem autoritativa, você pode usar suas próprias políticas de senha.</span><span class="sxs-lookup"><span data-stu-id="71726-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="71726-111">[Redefinir a senha de autoatendimento (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que usuários redefinam suas próprias senhas na nuvem ao ainda aplicar a política de senhas no local.</span><span class="sxs-lookup"><span data-stu-id="71726-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="71726-112">[Write-back de dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que os dispositivos registrados no Azure AD a serem gravados de volta ao Active Directory local para que possam ser usadas para acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="71726-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="71726-p104">[Impedir acidental exclusões](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) é habilitado por padrão para ajudar a impedir exclusões de objeto simultâneo de muitas (mais de 500 objetos por sincronização). Você pode alterar essa configuração para atender às necessidades da sua organização.</span><span class="sxs-lookup"><span data-stu-id="71726-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="71726-115">[Atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está habilitada por padrão para instalações express e ajuda a garantir que sua versão do Windows Azure Connect da AD é sempre atual.</span><span class="sxs-lookup"><span data-stu-id="71726-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

