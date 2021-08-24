---
title: Imagem do usuário não exibida no organograma do Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467363"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Imagem do usuário não exibida no organograma do Microsoft Teams

Se um ou mais indivíduos de sua organização não tiverem sua foto de perfil no organograma, é possível que a configuração **ShowInAddressLists** esteja definida como **Falso**:

1. Acesse o Centro de administração do Microsoft 365 > [**Usuários Ativos**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)e selecione o usuário com sem a foto. 
1. Selecione a guia **E-mail** certifique-se de que **Mostrar na lista de endereços global** esteja definido como **Sim**. 

Se a definição **ShowInAddressLists** como **Sim** não funcionar, verifique o seguinte:

- O usuário pode estar oculto na lista de destinatários no Exchange. Para obter mais informações, consulte [Gerenciar listas de endereços no Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- O usuário pode estar oculto da lista de endereços no Azure Active Directory. Para obter mais informações, consulte [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
