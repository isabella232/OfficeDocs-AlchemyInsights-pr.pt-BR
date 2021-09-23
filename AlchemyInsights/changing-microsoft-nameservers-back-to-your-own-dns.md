---
title: Alterar do nameservers da Microsoft de volta para gerenciar seus próprios registros DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481831"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Alterar do nameservers da Microsoft de volta para gerenciar seus próprios registros DNS

Anteriormente, você alterou seus registros NS para apontar para a Microsoft (ns1.bdm.microsoftonline.com), mas atualmente decidiu gerenciar seus próprios registros DNS:

No seu site do registrador de domínios, altere o nameserver de volta ao seu registrador ou configuração anterior. Se você não estiver familiarizado com o DNS, contate o suporte no registrador de domínio. Observe que as vezes as alterações do nameserver podem levar até 48 horas para serem propagadas. 

1. No portal de Administração do Microsoft 365, acesse **Configurações** > [**Domínios**](https://admin.microsoft.com/Adminportal/Home#/Domains), selecione a caixa de seleção ao lado do domínio e selecione **Gerenciar DNS**. 

2. No assistente, selecione **Adicionar seus próprios registros DNS** e conclua o assistente. Isso altera a maneira como o seu DNS é gerenciado e permite que você adicione os registros DNS personalizados necessários para dar suporte aos seus serviços selecionados.

Como alternativa, se você alterou seus registros do nameserver na Microsoft e possuir um site, você pode adicionar registros DNS ao site em vez de alterar os nameservers de volta. Para obter mais informações, consulte [Atualize os registros DNS para manter seu site com o provedor de hospedagem atual](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).


