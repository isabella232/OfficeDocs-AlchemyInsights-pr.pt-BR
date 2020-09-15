---
title: 646 como configurar o AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704477"
---
# <a name="configure-sync-features"></a>Configurar recursos de sincronização

O Azure AD Connect inclui vários recursos habilitados por padrão ou que você pode habilitar posteriormente. Alguns recursos exigem configuração adicional em ambientes específicos.

- [Filtrando](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limites os objetos estão sincronizados com o Azure AD. Por padrão, todos os usuários, contatos, grupos e contas de computador do Windows 10 são sincronizados. Você pode incluir ou excluir objetos com base em domínios, UOs ou outros atributos.

- A [sincronização de hash de senha](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de senha do Active Directory local para o Azure AD. Isso permite o gerenciamento de senhas em um local, mas o uso da mesma senha em ambientes locais e em nuvem. Como o Active Directory é a fonte autoritativa, você pode usar suas próprias diretivas de senha.

- [A redefinição de senha de autoatendimento (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que os usuários redefinam suas próprias senhas na nuvem enquanto ainda aplicam sua política de senha local.

- O [write-back de dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que dispositivos registrados no Azure ad sejam gravados novamente no Active Directory local para que possam ser usados para acesso condicional.

- [Impedir que exclusões acidentais](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) sejam habilitadas por padrão para ajudar a evitar muitas exclusões de objetos simultâneas (mais de 500 objetos por sincronização). Você pode alterar essa configuração para atender às necessidades da sua organização.

- A [atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está habilitada por padrão para instalações expressas e ajuda a garantir que sua versão do Azure ad Connect seja sempre atual.
