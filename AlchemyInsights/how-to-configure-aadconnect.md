---
title: 646 como configurar o AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399759"
---
# <a name="configure-sync-features"></a>Configurar recursos de sincronização

O Azure AD Connect inclui vários recursos habilitados por padrão ou que você pode habilitar posteriormente. Alguns recursos exigem configuração adicional em ambientes específicos.

- [Filtrando](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limites os objetos estão sincronizados com o Azure AD. Por padrão, todos os usuários, contatos, grupos e contas de computador do Windows 10 são sincronizados. Você pode incluir ou excluir objetos com base em domínios, UOs ou outros atributos.

- A [sincronização de hash de senha](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de senha do Active Directory local para o Azure AD. Isso permite o gerenciamento de senhas em um local, mas o uso da mesma senha em ambientes locais e em nuvem. Como o Active Directory é a fonte autoritativa, você pode usar suas próprias diretivas de senha.

- [A redefinição de senha de autoatendimento (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que os usuários redefinam suas próprias senhas na nuvem enquanto ainda aplicam sua política de senha local.

- O [write-back de dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que dispositivos registrados no Azure ad sejam gravados novamente no Active Directory local para que possam ser usados para acesso condicional.

- [Impedir que exclusões acidentais](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) sejam habilitadas por padrão para ajudar a evitar muitas exclusões de objetos simultâneas (mais de 500 objetos por sincronização). Você pode alterar essa configuração para atender às necessidades da sua organização.

- A [atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está habilitada por padrão para instalações expressas e ajuda a garantir que sua versão do Azure ad Connect seja sempre atual.
