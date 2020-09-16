---
title: Enviar notificações personalizadas com o Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720634"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="b5586-102">Como enviar notificações personalizadas para os usuários de dispositivos iOS e Android gerenciados</span><span class="sxs-lookup"><span data-stu-id="b5586-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="b5586-103">As notificações personalizadas para o Intune são processadas pelo aplicativo do portal da empresa no dispositivo de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b5586-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="b5586-104">Em seguida, o aplicativo cria a notificação por push nesse dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5586-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="b5586-105">Estes são os pré-requisitos de dispositivo para suportar o recebimento de notificações personalizadas e para o aplicativo criar a notificação por push:</span><span class="sxs-lookup"><span data-stu-id="b5586-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="b5586-106">O dispositivo deve ter o aplicativo portal da empresa instalado.</span><span class="sxs-lookup"><span data-stu-id="b5586-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="b5586-107">O dispositivo deve permitir que o aplicativo do portal da empresa envie notificações por push.</span><span class="sxs-lookup"><span data-stu-id="b5586-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="b5586-108">Quando o aplicativo é instalado ou atualizado, ele solicitará que o usuário permita notificações.</span><span class="sxs-lookup"><span data-stu-id="b5586-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="b5586-109">Os dispositivos Android devem ter o Google Play Services instalado.</span><span class="sxs-lookup"><span data-stu-id="b5586-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="b5586-110">O dispositivo deve ser inscrito no Intune.</span><span class="sxs-lookup"><span data-stu-id="b5586-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="b5586-111">Para obter mais informações, incluindo como enviar uma mensagem, consulte a [documentação do recurso](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="b5586-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
