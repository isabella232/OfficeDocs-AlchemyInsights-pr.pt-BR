---
title: Configuração virtual com serviços de domínio do AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884550"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Configuração virtual com serviços de domínio do AAD

A configuração virtual com serviços de domínio do AAD envolve as seguintes etapas: 

1. Verificar a integridade do domínio no portal do Azure https://aka.ms/aadds-health
2. Verificar o NSG em busca de regras que bloqueiam as portas necessárias para sincronizar o Azure Active Directory Domain Services ao portal https://aka.ms/aadds-networking
3. Garantir que a rede virtual seja implantada na mesma região do Azure que seu domínio gerenciado pelo Azure AD Domain Services.
4. Garantir que você não tenha um domínio existente com o mesmo nome de domínio disponível na rede virtual.

Para obter mais detalhes sobre a consideração de design na Rede Virtual do Azure para oferecer suporte a serviços de domínio do AAD, confira [Consideração sobre a Rede Virtual](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

