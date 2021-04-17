---
title: Centro de administração do Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826367"
---
# <a name="teams-admin-center"></a>Centro de administração do Teams

Saiba como gerenciar o Teams com o [Centro de Administração do Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Se você não conseguir acessar o Centro de Administração do Teams, verifique os seguintes itens:

- Verifique se você permitiu os [endereços IP e URLs apropriados do Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) em todos os dispositivos de perímetro (firewall, etc.) ou nas regras de firewall em seu computador local.
- Verifique se o logon que você está usando para acessar o Portal de Administração do Teams corresponde ao nome de usuário listado no [Portal de aAdministração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Se os usuários não estiverem aparecendo no Centro de Administração do Teams, confira o seguinte:

- Você criou usuários ou atribuiu licenças nas últimas 24 horas? Aguarde pelo menos 24 horas antes de abrir um tíquete de suporte.
- Verifique se você atribuiu licenças apropriadas.
- Se você tiver um Active Directory local, verifique se [o valor do msRTCSIP-PrimaryUserAddress ou o endereço SIP no campo ProxyAddresses no seu Active Directory local é único e o formato corresponde a](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)SIP:**Nome de usuário** do usuário do [Centro de administração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users). 
- Se você pretende manter uma implantação do Skype for Business Server e usuários estiverem hospedados no local e Online: vá em **"Configurar híbrido com o Teams e o Skype for Business Online"** no painel de controle do Skype for Business Server e mova os usuários Online.
