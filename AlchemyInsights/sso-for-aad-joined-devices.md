---
title: Single-Sign para dispositivos ingressados no Azure Active Directory
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
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403766"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Login único para dispositivos ingressados no Azure Active Directory

Se você tiver um ambiente local do Active Directory (AD) e quiser ingressar seus computadores ingressados no domínio do AD no Azure AD, poderá fazer isso fazendo a junção híbrida do Azure AD. Como planejar sua implementação de participação híbrida do [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) fornece as etapas relacionadas para implementar uma junção híbrida do Azure AD em seu ambiente.

[Configurar dispositivos ingressados no Azure AD para o Single-Sign local usando o Windows Hello para Empresas](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemas de PRT (Token** de Atualização Primária) Um Token de Atualização Principal (PRT) é um artefato-chave da autenticação do Azure AD no Windows 10, No Windows Server 2016 e versões posteriores, dispositivos iOS e Android. É um JSON Web Token (JWT) especialmente emitido para os corretores de token de primeira parte da Microsoft para habilitar o logon único (SSO) nos aplicativos usados nesses dispositivos. [Em O que é um Token de](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)Atualização Principal? , forneceremos detalhes sobre como uma PRT é emitida, usada e protegida em dispositivos Windows 10.

**WamDefaultSet: YES e AzureADPrt: SIM** Esses campos indicam se o usuário foi autenticado com êxito no Azure AD ao entrar no dispositivo. Se os valores são **NÃO,** pode ser devido:

- Chave de armazenamento ruim no TPM associada ao dispositivo durante o registro (verifique o KeySignTest durante a execução elevada).
- ID de Logon Alternativo
- Proxy HTTP não encontrado

Solucionar problemas de dispositivos usando o comando dsregcmd - [estado SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
