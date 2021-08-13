---
title: Problema com grupos de segurança
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
- "8252"
- "9004397"
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925729"
---
# <a name="issue-with-security-groups"></a>Problema com grupos de segurança

**Se você estiver recebendo o erro de rede AADDS104**

Regras de grupo de segurança de rede inválidas são a causa mais comum de erros de rede para os Serviços de Domínio Active Directory do Azure (AD DS). O grupo de segurança de rede para a rede virtual deve permitir o acesso a portas e protocolos específicos. Se essas portas estiverem bloqueadas, a plataforma Azure não poderá monitorar ou atualizar o domínio gerenciado. A sincronização entre o Azure AD e o Azure AD DS também é afetada. Certifique-se de manter as portas padrão abertas para evitar a interrupção do serviço.

Para compreender e resolver alertas comuns para problemas de configuração do grupo de segurança de rede, consulte [Adicionar e verificar grupos de segurança](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
