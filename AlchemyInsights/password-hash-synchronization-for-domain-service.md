---
title: Sincronização de hash de senha para serviço de domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162907"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sincronização de hash de senha para serviço de domínio

**Se sua instância do Azure AD DS estiver solicitando que você habilite a sincronização de hash de senha**

Você encontra um cenário no qual está executando um ambiente híbrido com usuários sincronizando a partir de um ambiente local dos Serviços de Domínio Active Directory (AD DS) do Azure. Este cenário é encontrado apesar de você ter sincronização de hash de senha do AD DS local para seu locatário do Microsoft Azure Active Directory.

**Causa**

Isso está acontecendo porque o Azure AD Connect, por padrão, não sincroniza o New Technology LAN Manager (NTLM) herdado e os hashes de senha Kerberos necessários para o Azure AD DS.

**Solução alternativa** 

Você precisaria configurar o Azure AD Connect para sincronizar os hashes de senha necessários para a autenticação NTLM e Kerberos.

Depois que o Azure AD Connect é configurado, uma criação de conta local ou evento de alteração de senha também sincroniza os hashes de senha herdados com o Azure AD. Consulte [aqui ](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) para obter mais informações sobre isso e para obter orientação sobre como habilitar a sincronização de senha em ambientes híbridos do Azure AD DS.