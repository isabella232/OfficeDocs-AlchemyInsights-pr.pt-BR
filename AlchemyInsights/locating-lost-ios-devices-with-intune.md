---
title: Localizando dispositivos iOS perdidos com o Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675143"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Localizando dispositivos iOS perdidos com o Intune

Habilitar o modo de perda em um dispositivo iOS permite que um administrador tenha uma mensagem e o número de telefone de contato exibido na tela de bloqueio.

Após o modo de perda ser habilitado, o administrador pode usar a ação localizar dispositivo para identificar o local físico do dispositivo.

A ação Localizar dispositivo no Intune funciona com dispositivos iOS para mostrar o local de um dispositivo específico em um mapa.

Usar essa ação requer que o dispositivo iOS esteja no:

- Modo supervisionado
- Modo perdido

Para saber mais, confira [Habilitar o modo perdido em dispositivos iOS/iPadOS com o Intune](https://docs.microsoft.com/intune/device-lost-mode) e [Localizar dispositivos iOS/iPadOS perdidos ou roubados com o Intune](https://docs.microsoft.com/intune/device-locate).

**Perguntas Frequentes**

P: Efetuei uma ação remota para remover dados da empresa de um dispositivo, mas agora ele está travado em um estado pendente.

R: Para que uma ação remota seja concluída com sucesso, o dispositivo de destino precisa estar online e íntegro. Nas situações a seguir, a ação remota permanece em um estado pendente por 30 dias ou até que o dispositivo confirme o comando:

- Quando o dispositivo não tem conectividade
- Quando o dispositivo perder seu status de gerenciamento com o Intune

Se você acha que um dispositivo não está mais fazendo check-in do e que não poderá remover dados da empresa, selecione Excluir. A exclusão irá remover o registro do dispositivo e ele não aparecerá mais na lista de dispositivos do Intune. Se o dispositivo se tornar ativo novamente, o usuário precisará registrá-lo novamente.

P: Por que determinadas ações remotas não estão disponíveis para uso?

R: Nem todas as plataformas são compatíveis com todas as ações remotas de dispositivos. As seguintes ações remotas são específicas de uma plataforma, para que elas fiquem disponíveis apenas para as plataformas indicadas.

- Ignorar bloqueio de ativação (somente iOS)
- Novo Início (somente Windows)
- Modo perdido (somente iOS)
- Localizar dispositivo (somente iOS)
- Reiniciar (somente Windows)

Para obter mais detalhes sobre cada uma dessas ações, confira o artigo [Ações disponíveis para dispositivos](https://docs.microsoft.com/intune/device-management#available-device-actions).