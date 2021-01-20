---
title: Configurar serviço de domínio
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884553"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Não é possível habilitar o AAD-DS ou a implantação está falhando

Para resolver o problema que faz com que o serviço de domínio do Azure AD (AAD-DS) não possa ser habilitado ou implantado, execute as seguintes etapas:

1. Se você estiver usando uma rede virtual já existente, verifique em seu NSG as regras que bloqueiam as portas necessárias para sincronizar o AAD-DS ao portal https://aka.ms/aadds-networking.
2. Verifique se a mensagem de erro foi respondida neste guia de solução de problemas que está disponível em https://aka.ms/aadds-troubleshoot-enable.
3. Tente implantar o Azure AD Domain Services em uma nova rede virtual.
4. Siga o guia de Introdução sobre como implantar o AAD-DS: [Criar e configurar o Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Se estiver tendo problemas com a implantação do Azure AD Domain Services, confira [Solucionar Problemas do Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) para resolver erros comuns e ajudá-lo a fazer as coisas funcionarem novamente. 

**Não é possível desabilitar o AAD-DS**

O AAD-DS não pode ser pausado. Se deseja parar de usar seu domínio gerenciado, ele deve ser excluído.
Para excluir seu domínio gerenciado, confira [Excluir serviço de domínio do Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



