---
title: Solucionar problemas de junção do Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939907"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Solucionar problemas de junção do Azure AD

1. Se [você estiver configurando](https://docs.microsoft.com/azure/active-directory/devices/overview) registros de dispositivo pela primeira vez, verifique se você analisou Introdução ao gerenciamento de dispositivos no Azure Active Directory que o orientará sobre como obter dispositivos sob o controle para o Azure AD. 
1. Se você estiver registrando dispositivos no Azure AD diretamente e registrando-os no Intune, você [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) precisará garantir que configurou o [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) e ter o licenciamento em vigor primeiro.
1. Verifique se você está autorizado a executar operações no Azure AD. Apenas um administrador global no Azure Active Directory pode gerenciar as configurações para registros de dispositivos.
1. Para fazer a implementação de ingressar no Azure AD, consulte [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Para obter mais detalhes sobre como resolver problemas comuns com a junção ao Azure AD, consulte Perguntas frequentes sobre o [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) e para o dispositivo Windows 10 pro, consulte Não é possível ingressar um computador do Windows 10 Pro no [Azure AD -](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) Precisa atualizar para – Microsoft Community
