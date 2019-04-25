---
title: Monitorar o acesso condicional
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418457"
---
# <a name="monitoring-conditional-access"></a>Monitorar o acesso condicional

Os usuários direcionados ao acesso condicional receberão um email de notificação se não atenderem aos requisitos de acesso da sua organização. Para resolver, recomendamos uma ou mais das seguintes soluções:
  
- Se presumir que o dispositivo esteja inscrito, recomende que o usuário acesse o aplicativo do portal da empresa e verifique se ele aparece no portal da empresa. Caso contrário, o usuário deverá registrar o dispositivo.
    
- No portal do Azure, vá para a **conformidade de dispositivo do Intune \> **. Em **monitorar** , clique em **conformidade de dispositivo**. Exiba o relatório de conformidade do dispositivo para verificar se o dispositivo do usuário está marcado como compatível. 
    
- No portal do Azure, vá para a **conformidade de dispositivo do Intune \> **. Em **gerenciar**, clique em **políticas**. Na lista de políticas de conformidade, verifique se um perfil foi atribuído ao dispositivo do usuário. Se nenhum perfil for atribuído, o Intune não conseguirá confirmar o status de conformidade do dispositivo. 
    
- Edite a atribuição de acesso condicional do usuário.
    
1. No portal do Azure, vá **para \> as políticas \> de acesso condicional do Intune**
    
2. Selecionar uma política na lista
    
3. Clique em **usuários e grupos**
    
4. Para direcionar uma determinada política em alguém, adicione-a à lista de **inclusões** . Para garantir que uma pessoa seja omitida da política, adicione-a à lista de **exclusão** . 
    
Leia mais: [como monitorar dispositivos de acesso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

