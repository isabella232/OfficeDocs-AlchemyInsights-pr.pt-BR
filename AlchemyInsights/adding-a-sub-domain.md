---
title: Adicionando um sub domínio
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475922"
---
# <a name="adding-a-sub-domain"></a>Adicionando um sub domínio

Os domínios sub podem ser adicionados ao mesmo ou a um locatário diferente do domínio pai. Em ambos os casos, você deve gerenciar suas próprias configurações de DNS no site do registrador. Se você tiver deixado a Microsoft gerenciar suas configurações de DNS com registros NS ou se você comprou o domínio da Microsoft, não poderá adicionar subdomas sem alterar isso primeiro.

Adicione primeiro o domínio pai e adicione o sub domínio. Se o subdomínio estiver no mesmo locatário, nenhuma verificação adicional será necessária. Se adicionar o sub domínio a um locatário separado, o registro txt DNS será necessário para verificação de propriedade antes de adicionar o domínio e os registros DNS adicionais para os serviços selecionados.

- Para adicionar um domínio ou subdomínio, siga o assistente [Adicionar Domínio](https://admin.microsoft.com/Adminportal#/Domains/Wizard)ou adicione o domínio ou subdomínio manualmente, indo para **Configuração**  >  **de Domínios**  >  **Adicionar domínio**.

Se necessário:

- Para alterar quem gerencia suas configurações de DNS para um domínio existente, vá para Configurações  >  [**Domínios,**](https://admin.microsoft.com/Adminportal/Home#/Domains)marque a caixa de seleção ao lado do domínio e selecione **Gerenciar DNS**. No assistente, selecione **Adicionar seus próprios registros DNS** e conclua o assistente.
- Para adicionar sub domínios a um domínio adquirido pela Microsoft, primeiro transfira o domínio para outro registrador e faça a alteração acima para gerenciar seus próprios registros DNS. Para obter instruções, [consulte Transfer a domain from Microsoft to another host](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Se você receber um erro de que seu domínio já está em uso por outros membros ou pessoas em sua organização, primeiro você precisará assumir essa conta não controlada antes de usar o domínio. Para obter instruções, [consulte Take over an unmanaged directory as administrator in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
