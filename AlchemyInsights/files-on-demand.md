---
title: Arquivos Sob Demanda
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406532"
---
# <a name="configure-files-on-demand"></a>Configurar Arquivos Sob Demanda

Os Arquivos do OneDrive Sob Demanda ajudam a acessar todos os arquivos no OneDrive sem precisar baixá-los nem usar o espaço de armazenamento do dispositivo.

Para configurar os Arquivos Sob Demanda em seu computador:

1. Selecione o ícone de nuvem branca ou azul do **OneDrive** na área de notificação da barra de tarefas do Windows. Selecione **Configurações e ajuda** ícone de engrenagem > **Configurações**.
2. Na guia **Configurações**, selecione a caixa **Economizar espaço e baixar os arquivos à medida que os usar**.  

Você também pode configurar os Arquivos Sob Demanda usando o registro.

Se você desabilitar essa configuração, os usuários do Windows 10 terão o mesmo comportamento de sincronização que os usuários de versões anteriores do Windows e não poderão ativar os Arquivos Sob Demanda. Se você não definir essa configuração, os usuários podem ativar ou desativar os Arquivos Sob Demanda.

Habilitar essa política define a seguinte chave do registro como 1. Desabilitar essa política define a seguinte chave do registro como 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Se não conseguir ver a opção Arquivos Sob Demanda em "Configurações", certifique-se de que o tipo de início do serviço "Driver de Filtro de Arquivos do Windows Cloud" esteja definido como 2 (AUTO_START). A habilitação deste recurso define o seguinte valor da chave do registro como 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`