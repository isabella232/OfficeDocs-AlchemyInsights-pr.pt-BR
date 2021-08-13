---
title: Problemas de desempenho SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093671"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários

Se um OneDrive ou SharePoint não estiver disponível para vários usuários que anteriormente tinham acesso, pode haver um problema de serviço temporário. [Verifique o painel de saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).

**Adicionar e licenciar o usuário**

Certifique-se de [atribuir licenças aos usuários no Microsoft 365 para empresas.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Atribuir permissões**

Se o usuário tiver recebido uma licença do Sharepoint e ainda estiver recebendo uma mensagem de acesso negada, verifique se ele tem o [nível](https://docs.microsoft.com/sharepoint/understanding-permission-levels) de permissão apropriado atribuído.

**Considere usar o recurso de solicitação de acesso**

O [recurso de solicitação de](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) acesso permite que as pessoas solicitem acesso ao conteúdo que não têm permissão para ver no momento.

**Permitir script personalizado pode causar problemas de acesso negados**

Há certos cenários em que o *recurso Permitir script personalizado* pode estar apresentando um acesso negado. Para uma lista de recursos afetados, considerações de segurança e a capacidade de desabilitar o recurso. Visite Permitir [ou impedir script personalizado.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

