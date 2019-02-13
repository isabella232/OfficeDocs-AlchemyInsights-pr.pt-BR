---
title: 646 como configurar AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: dd6d6986b23c8adcc98fe713bacf32fb5bf8b4b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915549"
---
# <a name="configure-sync-features"></a>Configurar recursos de sincronização

Conectar do Azure AD inclui vários recursos que estão habilitados por padrão, ou que você pode habilitar posteriormente. Alguns recursos exigem configuração adicional em ambientes específicos.
  
- Limites de [filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) os objetos são sincronizados para o Windows Azure AD. Por padrão, todos os usuários, contatos, grupos e Windows 10 contas de computador são sincronizadas. Você pode incluir ou excluir objetos com base em domínios, OUs ou outros atributos. 
    
- [Sincronização de hash de senha](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash da senha do Active Directory local para o Windows Azure AD. Isso permite que o gerenciamento de senha em um único local, mas o uso da mesma senha nos dois locais e ambientes em nuvem. Como o Active Directory é a origem autoritativa, você pode usar suas próprias políticas de senha. 
    
- [Redefinir a senha de autoatendimento (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que usuários redefinam suas próprias senhas na nuvem ao ainda aplicar a política de senhas no local. 
    
- [Write-back de dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que os dispositivos registrados no Azure AD a serem gravados de volta ao Active Directory local para que possam ser usadas para acesso condicional. 
    
- [Impedir acidental exclusões](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) é habilitado por padrão para ajudar a impedir exclusões de objeto simultâneo de muitas (mais de 500 objetos por sincronização). Você pode alterar essa configuração para atender às necessidades da sua organização. 
    
- [Atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está habilitada por padrão para instalações express e ajuda a garantir que sua versão do Windows Azure Connect da AD é sempre atual. 
    

