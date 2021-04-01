---
title: Definir o Microsoft Edge como o navegador padrão em um dispositivo ingressado em um domínio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426762"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Definir o Microsoft Edge como o navegador padrão em um dispositivo ingressado em um domínio

Definir Microsoft Edge como o navegador padrão: 

1. [Criar um arquivo de configuração de associações padrão](https://go.microsoft.com/fwlink/?linkid=2132437) e armazená-lo localmente ou em um compartilhamento de rede.

1. Abra o editor de Políticas de Grupo, e depois vá para **Configuração do Computador** > **Modelos Administrativos** > **Componentes do Windows** > **Explorador de Arquivos**.

1. Selecione **Configurar um arquivo padrão de configuração de associações**.

1. Selecione **Configuração de política**, e depois selecione **Habilitado**.

1. Em **Opções**, digite a localização do seu arquivo de configuração de associações padrão e selecione **OK**.
