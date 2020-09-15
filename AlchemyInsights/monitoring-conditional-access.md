---
title: Monitorar o acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702891"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorar o acesso condicional do Exchange

Os usuários direcionados ao acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:
  
- Se presumir que o dispositivo esteja inscrito, recomende que o usuário acesse o aplicativo do portal da empresa e verifique se ele aparece no portal da empresa. Caso contrário, o usuário deverá registrar o dispositivo.
    
- No portal do Azure, vá para a ** \> conformidade de dispositivo do Intune**. Em **monitorar** , clique em **conformidade de dispositivo**. Exiba o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como compatível. 
    
- No portal do Azure, vá para a ** \> conformidade de dispositivo do Intune**. Em **gerenciar**, clique em **políticas**. Na lista de políticas de conformidade, verifique se um perfil foi atribuído ao dispositivo do usuário. Se nenhum perfil for atribuído, o Intune não conseguirá confirmar o status de conformidade do dispositivo. 
    
- Edite a atribuição de acesso condicional do usuário.
    
1. No portal do Azure, vá **para \> \> as políticas de acesso condicional do Intune**
    
2. Selecionar uma política na lista
    
3. Clique em **usuários e grupos**
    
4. Para direcionar uma determinada política em alguém, adicione-a à lista de **inclusões** . Para garantir que uma pessoa seja omitida da política, adicione-a à lista de **exclusão** . 
    
Leia mais: [como monitorar dispositivos de acesso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

