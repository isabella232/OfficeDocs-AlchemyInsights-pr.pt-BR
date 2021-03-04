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
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416301"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Removendo dados e limpando dispositivos do Intune

As ações remotas de Apagamento do Dispositivo e Desativação de Dispositivo podem ser usadas para remover dados da empresa gerenciados pelo Intune ou para executar uma redefinição de fábrica e restaurar o dispositivo com as configurações padrão.

1. Entre no Gerenciamento de Dispositivo do Microsoft 365, e vá para **Dispositivos** > **Todos Dispositivos**.
2. Selecione o dispositivo que deseja apagar.
3. Selecione o tipo de apagamento remoto que deseja executar. A desativação exclui somente as informações organizacionais, enquanto as exclusões completas restauram o dispositivo para suas configurações de fábrica.
4. Selecione **Sim** para confirmar. Até que a limpeza seja concluída, o status de ação do dispositivo é mostrado como *Retire Pending*.
    Após a conclusão da ação, você não verá mais o dispositivo móvel na lista de dispositivos gerenciados.

> [!NOTE]
> Dados da empresa não podem ser removidos dos dispositivos UNIDOS ao Microsoft Azure Active Directory. 

Para obter detalhes completos sobre o efeito das ações Retirar e Limpar, incluindo o que é retido e o que é excluído, consulte a seguinte documentação:

- [Remova dispositivos limpando, retirando ou cancelando a inscrição manualmente](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Como limpar apenas dados corporativos de aplicativos gerenciados pelo Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Apague todos os dados de um dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).