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
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="f49aa-102">Login único para dispositivos ingressados no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f49aa-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="f49aa-103">Se você tiver um ambiente local do Active Directory (AD) e quiser ingressar seus computadores ingressados no domínio do AD no Azure AD, poderá fazer isso fazendo a junção híbrida do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f49aa-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="f49aa-104">Como planejar sua implementação de participação híbrida do [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) fornece as etapas relacionadas para implementar uma junção híbrida do Azure AD em seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="f49aa-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="f49aa-105">Configurar dispositivos ingressados no Azure AD para o Single-Sign local usando o Windows Hello para Empresas</span><span class="sxs-lookup"><span data-stu-id="f49aa-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="f49aa-106">**Problemas de PRT (Token** de Atualização Primária) Um Token de Atualização Principal (PRT) é um artefato-chave da autenticação do Azure AD no Windows 10, No Windows Server 2016 e versões posteriores, dispositivos iOS e Android.</span><span class="sxs-lookup"><span data-stu-id="f49aa-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="f49aa-107">É um JSON Web Token (JWT) especialmente emitido para os corretores de token de primeira parte da Microsoft para habilitar o logon único (SSO) nos aplicativos usados nesses dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f49aa-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="f49aa-108">[Em O que é um Token de](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)Atualização Principal? , forneceremos detalhes sobre como uma PRT é emitida, usada e protegida em dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f49aa-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="f49aa-109">**WamDefaultSet: YES e AzureADPrt: SIM** Esses campos indicam se o usuário foi autenticado com êxito no Azure AD ao entrar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f49aa-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="f49aa-110">Se os valores são **NÃO,** pode ser devido:</span><span class="sxs-lookup"><span data-stu-id="f49aa-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="f49aa-111">Chave de armazenamento ruim no TPM associada ao dispositivo durante o registro (verifique o KeySignTest durante a execução elevada).</span><span class="sxs-lookup"><span data-stu-id="f49aa-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="f49aa-112">ID de Logon Alternativo</span><span class="sxs-lookup"><span data-stu-id="f49aa-112">Alternate Login ID</span></span>
- <span data-ttu-id="f49aa-113">Proxy HTTP não encontrado</span><span class="sxs-lookup"><span data-stu-id="f49aa-113">HTTP Proxy not found</span></span>

<span data-ttu-id="f49aa-114">Solucionar problemas de dispositivos usando o comando dsregcmd - [estado SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="f49aa-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
