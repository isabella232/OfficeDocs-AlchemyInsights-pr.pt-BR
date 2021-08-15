---
title: Mitigar o erro O aplicativo não foi detectado
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026102"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Mitigar o erro "O aplicativo não foi detectado"

O erro de instalação de aplicativo "O aplicativo não foi detectado após a instalação bem-sucedida", relatado pelo Intune, pode ocorrer em todas as principais plataformas de sistema operacional (Windows, iOS e Android).

Os cenários mais comuns que geram esse erro incluem:

- O aplicativo foi atualizado fora do Intune (a partir de uma loja de aplicativos de terceiros) após a implantação inicial. Por exemplo, alguns aplicativos, como o Google Chrome, podem executar atualizações automáticas.
- Um usuário desinstalou o aplicativo após a instalação inicial.

Para corrigir esse problema, primeiro execute uma análise dos dispositivos afetados para determinar o cenário em que o erro ocorreu.

- Se o aplicativo tiver sido atualizado fora do Intune, a implantação de aplicativos poderá ser configurada para ignorar a versão do aplicativo. Para fazer isso, em **Configuração do Aplicativo > Informações do Aplicativo,**, defina **Ignorar versão do aplicativo** como **Sim**.
- Ao direcionar o cliente, pode ser apropriado implantar o aplicativo como "necessário", além de garantir que a versão mais recente tenha sido implantada.
- Como alternativa, na plataforma iOS, é possível usar a funcionalidade **AutoUpdate** associada ao Programa de Compra de Volume Apple, que pode ser configurada para atualizar automaticamente para novas versões do aplicativo à medida que elas são disponibilizadas.

Para obter mais informações sobre como solucionar problemas de instalação do aplicativo, confira [Solucionar problemas de instalação do aplicativo](https://docs.microsoft.com/intune/troubleshoot-app-install).
