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
# <a name="using-email-profiles-with-intune"></a>Usar perfis de email com o Intune

O Intune pode ser usado para criar e implantar perfis de email para o cliente de email nativo (interno) em várias plataformas de dispositivos.

Para obter informações sobre algumas das restrições associadas a perfis de email, incluindo como a presença de perfis existentes são tratados e como remover perfis de email, veja [Adicionar configurações de email aos dispositivos usando o Intune](https://docs.microsoft.com/intune/email-settings-configure).

Para saber mais sobre como criar perfis de email para cada plataforma de dispositivo, consulte:

[Configurações de dispositivo Android para configurar, autenticar e sincronizar email no Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Adicionar configurações de email a dispositivos iOS e iPadOS no Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Configurações de perfil de email no Microsoft Intune para dispositivos que executam o Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Configurações de perfil de email para dispositivos com Windows 10 no Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Problema comum de sincronização**

**Um KNOX no perfil de email do Android impede que contatos, calendário e tarefas do usuário sejam sincronizados com os dispositivos dos usuários.**

O KNOX no perfil de email do Android oferece ao administrador a opção de decidir quais tipos de conteúdo serão sincronizados com o dispositivo, configurando cada um como habilitado.

Se a configuração de qualquer um dos tipos de conteúdo estiver definida como **Não configurada** (o padrão), esse tipo de conteúdo não será sincronizado automaticamente. Um usuário pode habilitar o tipo de conteúdo desejado diretamente no dispositivo, manualmente, mas essa configuração é substituída pela configuração de política do Intune, e a sincronização é interrompida para esse tipo de conteúdo.

