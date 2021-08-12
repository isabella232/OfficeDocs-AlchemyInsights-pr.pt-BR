---
title: 646 Como configurar o AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963631"
---
# <a name="configure-sync-features"></a>Configurar recursos de sincronização

O Azure AD Conexão inclui vários recursos habilitados por padrão ou que você pode habilitar posteriormente. Alguns recursos exigem configuração adicional em ambientes específicos.

- [Limites de](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) filtragem os objetos são sincronizados com o Azure AD. Por padrão, todos os usuários, contatos, grupos e Windows 10 contas de computador são sincronizadas. Você pode incluir ou excluir objetos com base em domínios, OUs ou outros atributos.

- [A sincronização de hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) de senha sincroniza o hash de senha do Active Directory local para o Azure AD. Isso permite o gerenciamento de senhas em um local, mas o uso da mesma senha em ambientes locais e de nuvem. Como o Active Directory é a fonte autoritativa, você pode usar suas próprias políticas de senha.

- A redefinição de senha de autoatendados [(SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que os usuários redefinir suas próprias senhas na nuvem enquanto ainda aplicam sua política de senha local.

- [O writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) de dispositivo permite que dispositivos registrados no Azure AD sejam gravados no Active Directory local para que possam ser usados para acesso condicional.

- [A prevenção de exclusões](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) acidentais é habilitada por padrão para ajudar a evitar muitas exclusões simultâneas de objetos (mais de 500 objetos por sincronização). Você pode alterar essa configuração para atender às necessidades da sua organização.

- [A atualização](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) automática é habilitada por padrão para instalações expressas e ajuda a garantir que sua versão do Azure AD Conexão sempre atual.
