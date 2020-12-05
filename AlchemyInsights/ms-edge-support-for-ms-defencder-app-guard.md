---
title: Suporte da Microsoft para o Microsoft defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576355"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Suporte da Microsoft para o Microsoft defender Application Guard

Projetado para o Windows 10 e o Microsoft Edge, o Application Guard usa uma abordagem de isolamento de hardware que permite que um usuário navegue em um site não confiável de dentro de um contêiner isolado, Hyper-V –, separado do sistema operacional host.

Um administrador corporativo define uma lista de sites confiáveis, recursos de nuvem e redes internas. Quando um usuário visita um site que não está na lista, o Microsoft Edge abrirá o site no contêiner. Isso significa que, se o site for mal-intencionado, o computador host permanecerá protegido e o invasor não receberá os dados da empresa.

A instalação de extensões no contêiner tem suporte da versão 81 do Microsoft Edge e pode ser controlada por uma política. O endereço updateURL que é usado na política ExtensionInstallForcelist deve ser adicionado como um recurso neutro nas diretivas de isolamento de rede usadas pelo Application Guard.

Para obter mais informações, consulte [suporte do Microsoft Edge para o Microsoft defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
