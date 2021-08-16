---
title: Sincronização de serviço de domínio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: 95b5c3b768caf4b5d80a088a17a33facb39805fc766e4888586ae052d91681e3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057846"
---
# <a name="domain-service-synchronization"></a>Sincronização de serviço de domínio

Objetos e credenciais em um domínio gerenciado dos Serviços de Domínio Azure Active Directory (Azure AD DS) podem ser criados localmente dentro do domínio ou sincronizados de um locatário do Azure Active Directory (Azure AD). Quando você implanta pela primeira vez o Azure AD DS, uma sincronização automática de ida e volta é configurada e iniciada para replicar os objetos do Azure AD. Essa sincronização única continua sendo executado em segundo plano para manter o domínio gerenciado do Azure AD DS atualizado com quaisquer alterações do Azure AD. Nenhuma sincronização ocorre do Azure AD DS de volta para o Azure AD.

Para obter mais detalhes sobre Azure Active Directory de serviço de domínio, consulte [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization). 
