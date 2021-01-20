---
title: 'Controlador de domínio '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886768"
---
# <a name="domain-controller"></a>Controlador de domínio

**Não é possível habilitar o AAD-DS ou a implantação está falhando**

Para resolver o problema que faz com que o serviço de domínio do Azure Active Directory (AAD-DS) não possa ser habilitado ou implantado, execute as seguintes etapas:

1. Se você estiver usando uma rede virtual já existente, verifique em seu NSG as regras que bloqueiam as portas necessárias para sincronizar o AAD-DS ao portal https://aka.ms/aadds-networking.
2. Verifique se a mensagem de erro foi respondida neste guia de solução de problemas que está disponível em  https://aka.ms/aadds-troubleshoot-enable.
3. Tente implantar o Azure AD Domain Services em uma nova rede virtual.
4. Siga o guia de Introdução sobre como implantar o AAD-DS, que está disponível no [Tutorial para Criar Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Se estiver tendo problemas com a implantação do Azure AD Domain Services, consulte [Solucionar problemas do Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) para resolver erros comuns e ajudá-lo a fazer as coisas funcionarem novamente. 

**Não é possível desabilitar o AAD-DS**

O AAD-DS não pode ser pausado. Se deseja parar de usar seu domínio gerenciado, ele deve ser excluído.

Se você tiver problemas para resolver mensagens de erro comuns e para etapas de solução de problemas associadas para ajudá-lo a voltar a funcionar, consulte [Solucionar problemas do Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
