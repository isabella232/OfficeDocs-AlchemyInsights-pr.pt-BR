---
title: Configurar LDAP
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
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090400"
---
# <a name="configure-ldap"></a>Configurar LDAP

Para configurar o LDAP, faça o seguinte:

1. Verifique a saúde do seu domínio no [portal do Azure.](https://aka.ms/aadds-health)
1. Verifique se uma assinatura válida do Azure AD está disponível e os Serviços de Domínio do Azure AD foram habilitados.
1. O certificado necessário para habilitar o LDAP seguro deve ser obtido de uma autoridade de certificação pública confiável ou ser um certificado auto-assinado.
1. Verifique se o certificado segue as [diretrizes necessárias.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Certificado Inválido**
1. Para renovar um certificado, siga as etapas para criar um novo certificado e recarregar: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Para resolver um problema conhecido com alertas LDAP seguros nos Serviços de Domínio do Azure Active directory, consulte [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
