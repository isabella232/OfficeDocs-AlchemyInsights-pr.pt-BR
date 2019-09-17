---
title: Enviar notificações personalizadas com o Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992301"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="a98d4-102">Como enviar notificações personalizadas para os usuários de dispositivos iOS e Android gerenciados</span><span class="sxs-lookup"><span data-stu-id="a98d4-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="a98d4-103">As notificações personalizadas para o Intune são processadas pelo aplicativo do portal da empresa no dispositivo de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a98d4-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="a98d4-104">Em seguida, o aplicativo cria a notificação por push nesse dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a98d4-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="a98d4-105">Estes são os pré-requisitos de dispositivo para suportar o recebimento de notificações personalizadas e para o aplicativo criar a notificação por push:</span><span class="sxs-lookup"><span data-stu-id="a98d4-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="a98d4-106">O dispositivo deve ter o aplicativo portal da empresa instalado.</span><span class="sxs-lookup"><span data-stu-id="a98d4-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="a98d4-107">O dispositivo deve permitir que o aplicativo do portal da empresa envie notificações por push.</span><span class="sxs-lookup"><span data-stu-id="a98d4-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="a98d4-108">Quando o aplicativo é instalado ou atualizado, ele solicitará que o usuário permita notificações.</span><span class="sxs-lookup"><span data-stu-id="a98d4-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="a98d4-109">Os dispositivos Android devem ter o Google Play Services instalado.</span><span class="sxs-lookup"><span data-stu-id="a98d4-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="a98d4-110">O dispositivo deve ser inscrito no Intune.</span><span class="sxs-lookup"><span data-stu-id="a98d4-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="a98d4-111">Para obter mais informações, incluindo como enviar uma mensagem, consulte a [documentação do recurso](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="a98d4-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
