---
title: Removendo dados e limpando dispositivos do Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701271"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Removendo dados e limpando dispositivos do Intune

As ações remotas de Apagamento do Dispositivo e Desativação de Dispositivo podem ser usadas para remover dados da empresa gerenciados pelo Intune ou para executar uma redefinição de fábrica e restaurar o dispositivo com as configurações padrão.

1. Entre no Gerenciamento de Dispositivo do Microsoft 365, e vá para **Dispositivos** > **Todos Dispositivos**.
2. Selecione o dispositivo que deseja apagar.
3. Selecione o tipo de apagamento remoto que deseja executar. A desativação exclui somente as informações organizacionais, enquanto as exclusões completas restauram o dispositivo para suas configurações de fábrica.
4. Selecione **Sim** para confirmar. Até que o apagamento seja concluído, o status da ação do Dispositivo é mostrado como Desativação Pendente.</br>
    Após a conclusão da ação, você não verá mais o dispositivo móvel na lista de dispositivos gerenciados.

**Observação** Dados da empresa não podem ser removidos de dispositivos ASSOCIADOS ao Azure AD.

Para detalhes completos sobre o efeito das ações de Desativar e Apagar, incluindo o que é mantido e o que é excluído, confira [Remover dispositivos usando apagar, desativar ou manualmente cancelar o registro do dispositivo](https://docs.microsoft.com/intune/devices-wipe).

Para apagar todos os dados de um dispositivo macOS, confira [Apagar todos os dados de um dispositivo macOS](https://docs.microsoft.com/intune/device-erase).