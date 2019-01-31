---
title: Monitoramento de acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656555"
---
# <a name="monitoring-conditional-access"></a>Monitoramento de acesso condicional

Usuários visados com acesso condicional receberá um email de notificação, se elas não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:
  
- Se o dispositivo é provável que será registrado, avisa o usuário ir para o aplicativo de Portal da empresa e verifique se ele aparece no Portal de empresa. Caso contrário, o usuário deve registrar o dispositivo.
    
- No portal do Azure, vá para **Intune \> conformidade de dispositivo**. Em **Monitor** , clique em **conformidade do dispositivo**. Exiba o relatório de conformidade do dispositivo para verificar que o dispositivo do usuário está marcado como compatível. 
    
- No portal do Azure, vá para **Intune \> conformidade de dispositivo**. Em **Gerenciar**, clique em **políticas**. Na lista de políticas de conformidade, verifique se um perfil é atribuído ao dispositivo do usuário. Se nenhum perfil for atribuída, Intune não poderá confirmar o status de conformidade do dispositivo. 
    
- Edite a atribuição de condicional de acesso do usuário.
    
1. No portal do Azure, vá para **Intune \> acesso condicional \> políticas**
    
2. Selecione uma política na lista
    
3. Clique em **usuários e grupos**
    
4. Para direcionar a uma determinada política no alguém, adicioná-los à lista de **inclusão** . Para garantir que uma pessoa for omitida da diretiva, adicioná-los à lista de **exclusões** . 
    
Leia mais: [como condicional monitore o acesso de dispositivos](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

