---
title: Centro de administração do Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670352"
---
# <a name="teams-admin-center"></a><span data-ttu-id="d1dbf-102">Centro de administração do Teams</span><span class="sxs-lookup"><span data-stu-id="d1dbf-102">Teams Admin Center</span></span>

<span data-ttu-id="d1dbf-103">Saiba como gerenciar o Teams com o [Centro de Administração do Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="d1dbf-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="d1dbf-104">Se você não conseguir acessar o Centro de Administração do Teams, verifique os seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="d1dbf-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="d1dbf-105">Verifique se você permitiu os [endereços IP e URLs apropriados do Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) em todos os dispositivos de perímetro (firewall, etc.) ou nas regras de firewall em seu computador local.</span><span class="sxs-lookup"><span data-stu-id="d1dbf-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="d1dbf-106">Verifique se o logon que você está usando para acessar o Portal de Administração do Teams corresponde ao nome de usuário listado no [Portal de aAdministração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="d1dbf-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="d1dbf-107">Se os usuários não estiverem aparecendo no Centro de Administração do Teams, confira o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d1dbf-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="d1dbf-108">Você criou usuários ou atribuiu licenças nas últimas 24 horas?</span><span class="sxs-lookup"><span data-stu-id="d1dbf-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="d1dbf-109">Aguarde pelo menos 24 horas antes de abrir um tíquete de suporte.</span><span class="sxs-lookup"><span data-stu-id="d1dbf-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="d1dbf-110">Verifique se você atribuiu licenças apropriadas.</span><span class="sxs-lookup"><span data-stu-id="d1dbf-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="d1dbf-111">Se você tiver um Active Directory local, verifique se [o valor do msRTCSIP-PrimaryUserAddress ou o endereço SIP no campo ProxyAddresses no seu Active Directory local é único e o formato corresponde a ](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)SIP:**Nome de usuário** do usuário do [Centro de administração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users). </span><span class="sxs-lookup"><span data-stu-id="d1dbf-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="d1dbf-112">Se você pretende manter uma implantação do Skype for Business Server e usuários estiverem hospedados no local e Online: vá em **"Configurar híbrido com o Teams e o Skype for Business Online"** no painel de controle do Skype for Business Server e mova os usuários Online.</span><span class="sxs-lookup"><span data-stu-id="d1dbf-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
