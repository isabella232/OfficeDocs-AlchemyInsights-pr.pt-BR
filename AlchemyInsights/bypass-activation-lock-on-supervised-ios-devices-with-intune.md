---
title: Ignorar o bloqueio de ativação em dispositivos iOS supervisionados com o Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397691"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Ignorar o bloqueio de ativação em dispositivos iOS supervisionados com o Intune

A capacidade de ignorar o bloqueio de ativação nos dispositivos iOS torna mais fácil a recuperação de uma situação na qual um usuário habilita a ativação do bloqueio em um dispositivo corporativo e, em seguida, sai da empresa.

Os pré-requisitos para se ignorar uma ativação de bloqueio incluem:

- Um dispositivo que seja “supervisionado”.
- Um bloqueio de ativação habilitado com sucesso usando a política de restrições de dispositivos iOS no Intune.

Além disso, ao ignorar um bloqueio de ativação você deve:

- Ter em mãos (posse física) o dispositivo que está sendo apagado.
- Copiar o código antes de efetivar o apagamento.

**Observação:** o código de apagamento não diferencia maiúsculas e minúsculas e, portanto, os caracteres "-" não são necessários.

Para obter mais detalhes, confira o artigo [Ignorar bloqueios de ativação em dispositivos iOS supervisionados com o Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Perguntas Frequentes**

P: **Efetuei uma ação remota para remover dados da empresa de um dispositivo, mas agora ele está travado em um estado pendente.**

R: Para que uma ação remota seja concluída com sucesso, o dispositivo de destino precisa estar online e íntegro. Nas situações a seguir, a ação remota permanece em estado pendente por 30 dias ou até que o dispositivo confirme o comando, sempre que o dispositivo:

- Estiver sem conexão.
- Perder seu status de gerenciamento no Intune.

Se você acredita que um dispositivo não está mais tendo acesso e não será capaz de remover os dados da empresa, selecione Excluir. A exclusão irá remover o registro do dispositivo e ele não aparecerá mais na lista de dispositivos do Intune. Para que o dispositivo se torne ativo novamente, seu usuário precisará recadastrá-lo.

P: **Por que determinadas ações remotas não estão disponíveis para uso?**

R: Nem todas as plataformas são compatíveis com todas as ações remotas de dispositivos. As ações remotas a seguir são específicas para uma plataforma:

- Ignorar bloqueio de ativação (somente iOS)
- Novo Início (somente Windows)
- Modo perdido (somente iOS)
- Localizar dispositivo (somente iOS)
- Reiniciar (somente Windows)

Para obter mais detalhes sobre cada uma dessas ações, confira o artigo [Ações disponíveis para dispositivos](https://docs.microsoft.com/intune/device-management#available-device-actions).