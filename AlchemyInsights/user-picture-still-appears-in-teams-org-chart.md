---
title: A imagem do usuário ainda aparece no organograma do Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334348"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>A imagem do usuário ainda aparece no organograma do Microsoft Teams

Se uma ou mais pessoas em sua organização tiverem sido desabilitadas ou removidas e sua foto de perfil ainda aparecer no organograma, é possível que a configuração **ShowInAddressLists** esteja definida como Falso: 

1. Vá para o Centro de administração do Microsoft 365 > [Usuários Ativos](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) e selecione o usuário com a foto que ainda aparece. 
1. Selecione a guia **E-mail** e certifique-se de que **Mostrar na lista de endereços global** esteja definido como **Não**.

Se a configuração **ShowInAddressLists** como **Não** não funcionar, verifique o seguinte: 

- O usuário pode ser mostrado na lista de destinatários no Exchange. Para obter mais informações, consulte [Gerenciar listas de endereços no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- O usuário pode ser mostrado na lista de endereços Azure Active Directory. Para obter mais informações, consulte [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 