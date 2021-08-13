---
title: Atualizar registros DNS para manter seu site com seu provedor de hospedagem atual
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007670"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atualizar registros DNS para manter seu site com seu provedor de hospedagem atual

1. Na Centro de administração do Microsoft 365, vá para a página Domínios de Instalação e, na lista de domínios, selecione o domínio que  >  [](https://admin.microsoft.com/Adminportal#/Domains) você está usando para seu site.

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
