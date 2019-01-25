---
title: Atualizar registros DNS para manter seu site com seu provedor de hospedagem atual
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457072"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atualizar registros DNS para manter seu site com seu provedor de hospedagem atual

1. Na página [Domínios](https://portal.office.com/adminportal/home#/Domains), selecione o domínio que você usa para o site na lista de domínios e selecione **Configurações de DNS**, no Painel Gerenciamento. 
    
2. Selecione **+ Novo registro personalizado** e insira o seguinte: 
    
  - Para **Tipo DNS**, insira: **A (Endereço)**
    
  - Para **Nome do host ou Alias**, digite o seguinte: **@**
    
  - Para o **Endereço IP**, digite o endereço IP estático no qual seu site está hospedado no momento (por exemplo, 172.16.140.1). 
    
    Esse deve ser um endereço IP  *estático*  do site e não um endereço IP  *dinâmico*  . Verifique com o site o local de hospedagem do seu site para garantir que você pode obter um endereço IP estático para o site público. 
    
3. Selecione **Salvar**. 
    
Além disso, você pode criar um registro CNAME para ajudar os clientes a encontrarem seu site.
  
1. Selecione **+ Novo registro personalizado** e insira o seguinte: 
    
  - Para **Tipo DNS**, insira: **CNAME (Alias)**
    
  - Para **Nome do host ou Alias**, digite: **www**
    
  - Em **Pontos de endereçamento**, digite o FQDN (nome de domínio totalmente qualificado) do seu site (por exemplo, contoso.com). 
    
2. Selecione **Salvar**. 
    

