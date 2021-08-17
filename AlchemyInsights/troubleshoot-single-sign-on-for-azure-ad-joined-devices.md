---
title: Solucionar problemas de entrada única para dispositivos ingressados no Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039234"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Solucionar problemas de entrada única para dispositivos ingressados no Azure AD

Se você tiver um ambiente local do Active Directory (AD) e quiser ingressar seus computadores ingressados no domínio do AD no Azure AD, poderá fazer isso fazendo a junção híbrida do Azure AD. [Como planejar sua implementação de](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) Azure Active Directory de junção híbrida fornece as etapas relacionadas para implementar uma junção híbrida do Azure AD em seu ambiente.

Para obter mais informações, consulte [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Problemas de PRT (Token de Atualização Primária)**

Um Token de Atualização Principal (PRT) é um artefato-chave da autenticação do Azure AD em dispositivos Windows 10, Windows Server 2016 e versões posteriores, iOS e Android. É um JSON Web Token (JWT) especialmente emitido para os corretores de token de primeira parte da Microsoft para habilitar o logon único (SSO) nos aplicativos usados nesses dispositivos. Para obter detalhes sobre como uma PRT é emitida, usada e protegida em Windows 10 dispositivos, consulte O que é [um Token de Atualização Principal?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES e AzureADPrt: SIM**

Esses campos indicam se o usuário foi autenticado com êxito no Azure AD ao entrar no dispositivo. Se os valores são **NÃO**, pode ser devido a:

- Chave de armazenamento ruim no TPM associada ao dispositivo durante o registro (verifique o KeySignTest durante a execução elevada)
- ID de Logon Alternativo
- Proxy HTTP não encontrado

Para solucionar problemas de dispositivos usando o comando dsregcmd, consulte [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
