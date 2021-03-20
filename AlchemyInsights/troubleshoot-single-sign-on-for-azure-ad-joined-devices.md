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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897411"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="6f3c7-102">Solucionar problemas de entrada única para dispositivos ingressados no Azure AD</span><span class="sxs-lookup"><span data-stu-id="6f3c7-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="6f3c7-103">Se você tiver um ambiente local do Active Directory (AD) e quiser ingressar seus computadores ingressados no domínio do AD no Azure AD, poderá fazer isso fazendo a junção híbrida do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f3c7-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="6f3c7-104">Como planejar sua implementação de participação híbrida do [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) fornece as etapas relacionadas para implementar uma junção híbrida do Azure AD em seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="6f3c7-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="6f3c7-105">Para obter mais informações, consulte [Configure Azure AD joined devices for On premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="6f3c7-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="6f3c7-106">**Problemas de PRT (Token de Atualização Primária)**</span><span class="sxs-lookup"><span data-stu-id="6f3c7-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="6f3c7-107">Um Token de Atualização Principal (PRT) é um artefato-chave da autenticação do Azure AD no Windows 10, No Windows Server 2016 e versões posteriores, dispositivos iOS e Android.</span><span class="sxs-lookup"><span data-stu-id="6f3c7-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="6f3c7-108">É um JSON Web Token (JWT) especialmente emitido para os corretores de token de primeira parte da Microsoft para habilitar o logon único (SSO) nos aplicativos usados nesses dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6f3c7-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="6f3c7-109">Para obter detalhes sobre como uma PRT é emitida, usada e protegida em dispositivos Windows 10, consulte [O que é um Token de Atualização Principal?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="6f3c7-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="6f3c7-110">**WamDefaultSet: YES e AzureADPrt: SIM**</span><span class="sxs-lookup"><span data-stu-id="6f3c7-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="6f3c7-111">Esses campos indicam se o usuário foi autenticado com êxito no Azure AD ao entrar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f3c7-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="6f3c7-112">Se os valores são **NÃO**, pode ser devido a:</span><span class="sxs-lookup"><span data-stu-id="6f3c7-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="6f3c7-113">Chave de armazenamento ruim no TPM associada ao dispositivo durante o registro (verifique o KeySignTest durante a execução elevada)</span><span class="sxs-lookup"><span data-stu-id="6f3c7-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="6f3c7-114">ID de Logon Alternativo</span><span class="sxs-lookup"><span data-stu-id="6f3c7-114">Alternate Login ID</span></span>
- <span data-ttu-id="6f3c7-115">Proxy HTTP não encontrado</span><span class="sxs-lookup"><span data-stu-id="6f3c7-115">HTTP Proxy not found</span></span>

<span data-ttu-id="6f3c7-116">Para solucionar problemas de dispositivos usando o comando dsregcmd, consulte [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="6f3c7-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
