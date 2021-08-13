---
title: Mapeamento de atributo de provisionamento do usuário
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 73da476cc5913a16911839a59b80959d3c99a8bc22471febe421b022ce2c49ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918131"
---
# <a name="user-provisioning-attribute-mapping"></a>Mapeamento de atributo de provisionamento do usuário

1. Para solucionar problemas conhecidos de mapeamento de atributo, consulte [Mapeamentos de atributo](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. O Microsoft Azure Active Directory (AD) oferece suporte ao provisionamento do usuário para aplicativos SaaS de terceiros, como o Salesforce, G Suite e outros. Se você habilitar o provisionamento do usuário para um aplicativo SaaS de terceiros, o portal do Azure controlará seus valores de atributo por meio de mapeamentos de atributo. Para saber como personalizar os mapeamentos de atributo padrão, confira [Personalizar mapeamentos de atributo de provisionamento de usuário para aplicativos SaaS no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Para saber mais sobre o provisionamento de usuários do aplicativo SaaS, confira [O que é o provisionamento automático do usuário do aplicativo SaaS no Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning). 
3. Ao personalizar mapeamentos de atributo para provisionamento do usuário, você pode descobrir que o atributo que você deseja mapear não aparece na lista de atributos de Origem. O artigo [Sincronizar um atributo do seu Active Directory local para o Azure AD para provisionar um aplicativo](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) mostra como adicionar o atributo ausente sincronizando-o do seu AD local para o Azure AD.
