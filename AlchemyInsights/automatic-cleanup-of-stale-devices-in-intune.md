---
title: Limpeza automática de dispositivos obsoletos no Intune
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
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715009"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Limpeza automática de dispositivos obsoletos no Intune

O Intune permite que o administrador configure um intervalo de tempo entre 90 e 270 dias, após o qual os dispositivos obsoletos serão removidos do serviço. Essa configuração é em toda a organização e ativa o efeito imediatamente. Todos os dispositivos não verificados no servidor do Intune por um período que exceda a configuração serão excluídos permanentemente.

**Observação** Apenas objetos de dispositivo MDM estão qualificados para essa ação de limpeza. Os objetos de dispositivo apenas EAS são excluídos.

Para saber mais sobre quando um dispositivo fica qualificado para exclusão com base na configuração de limpeza do dispositivo e em seu "estado":

Configuração: **Excluir dispositivos após a última data de check-in: Sim (algum valor (N) em dias especificado)**

- Com base no valor (N) definido na configuração, o serviço do Intune excluirá o dispositivo na última vez em que ele fizer check-in.

Configuração: **Excluir dispositivos após a última data de check-in: Não**

- 180 dias após o certificado do dispositivo expirar e não for renovado, o dispositivo será excluído.

**Observação** Em ambos os casos, o dispositivo deve ser registrado com êxito no Intune. O registro ocorre durante o primeiro check-in de dispositivo com o serviço do Intune.

Se um dispositivo se inscrever com êxito para o Intune, mas não se tornar registrado em Intune, o dispositivo será excluído 270 dias após o registro. (90 dias para marcar o dispositivo como revogado e, em seguida, outro 180 dias para excluir o registro.)

No momento, não existe nenhum mecanismo no console do Intune para estabelecer a data de vencimento da certificação de dispositivos para um determinado dispositivo.