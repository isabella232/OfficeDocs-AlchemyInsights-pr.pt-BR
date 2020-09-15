---
title: Usar perfis de email com o Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653276"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="45241-102">Usar perfis de email com o Intune</span><span class="sxs-lookup"><span data-stu-id="45241-102">Using email profiles with Intune</span></span>

<span data-ttu-id="45241-103">O Intune pode ser usado para criar e implantar perfis de email para o cliente de email nativo (interno) em várias plataformas de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="45241-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="45241-104">Para obter informações sobre algumas das restrições associadas a perfis de email, incluindo como a presença de perfis existentes são tratados e como remover perfis de email, veja [Adicionar configurações de email aos dispositivos usando o Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="45241-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="45241-105">Para saber mais sobre como criar perfis de email para cada plataforma de dispositivo, consulte:</span><span class="sxs-lookup"><span data-stu-id="45241-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="45241-106">Configurações de dispositivo Android para configurar, autenticar e sincronizar email no Intune</span><span class="sxs-lookup"><span data-stu-id="45241-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="45241-107">Adicionar configurações de email a dispositivos iOS e iPadOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="45241-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="45241-108">Configurações de perfil de email no Microsoft Intune para dispositivos que executam o Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="45241-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="45241-109">Configurações de perfil de email para dispositivos com Windows 10 no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="45241-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="45241-110">**Problema comum de sincronização**</span><span class="sxs-lookup"><span data-stu-id="45241-110">**Common syncing issue**</span></span>

<span data-ttu-id="45241-111">**Um KNOX no perfil de email do Android impede que contatos, calendário e tarefas do usuário sejam sincronizados com os dispositivos dos usuários.**</span><span class="sxs-lookup"><span data-stu-id="45241-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="45241-112">O KNOX no perfil de email do Android oferece ao administrador a opção de decidir quais tipos de conteúdo serão sincronizados com o dispositivo, configurando cada um como habilitado.</span><span class="sxs-lookup"><span data-stu-id="45241-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="45241-113">Se a configuração de qualquer um dos tipos de conteúdo estiver definida como **Não configurada** (o padrão), esse tipo de conteúdo não será sincronizado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="45241-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="45241-114">Um usuário pode habilitar o tipo de conteúdo desejado diretamente no dispositivo, manualmente, mas essa configuração é substituída pela configuração de política do Intune, e a sincronização é interrompida para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="45241-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

