---
title: Solução de problemas do monitor existente
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2ecfb4e90f2d58654ec43a35e901ea4421e0e94fa95995ef890abc8af2d99ec7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981065"
---
# <a name="troubleshoot-an-existing-monitor"></a>Solucionar problemas de um monitor existente

Experimente essas soluções para solucionar problemas de um monitor. 

**Atualize a exibição do monitor:**

Pressione as seguintes teclas ao mesmo tempo: Windows Tecla + Ctrl + Shift + B. Isso atualizará a comunicação com o driver gráfico. Seus monitores piscarão momentaneamente e voltarão depois de alguns segundos.

**Solucionar problemas de hardware de monitoramento:**

1. Desconectar o cabo conectando seu computador ao monitor e conectá-lo novamente.
2. Desconecte os dispositivos não essenciais do computador (como adaptadores ou encaixes).

**Se você instalou recentemente uma atualização em seu computador, poderá reverter o driver de exibição:**

1. Selecione **Iniciar**, digite **gerenciador de dispositivos** e selecione Gerenciador de **Dispositivos** nos resultados.
2. Expanda **a seção Adaptadores de exibição,** clique com o botão direito do mouse no adaptador de exibição e selecione **Propriedades**.
3. Navegue até a guia **Driver** e selecione **Reverter Driver**. <br>
Observação: se isso não estiver disponível ou estiver acinzado, selecione **Não** nas opções abaixo para mover para a próxima etapa.
4. Talvez seja necessário reiniciar o computador antes que essas alterações entre em vigor.

**Desinstalar e reinstalar o driver de exibição:**

1. Selecione **Iniciar**, digite **gerenciador de dispositivos** e selecione Gerenciador de **Dispositivos** nos resultados.
2. Expanda **a seção Adaptadores de exibição,** clique com o botão direito do mouse no adaptador de exibição e selecione **Desinstalar o dispositivo**. 
3. Selecione a caixa ao lado de **Excluir o software de driver deste dispositivo** e selecione **Desinstalar**.<br>
Observação: você pode ser solicitado a reiniciar seu computador neste estágio. Certifique-se de anotar as instruções restantes antes de reiniciar.
4. Abra o Gerenciador de Dispositivos novamente.
5. Expanda **a seção Adaptadores de exibição,** clique com o botão direito do mouse no adaptador de exibição e selecione Atualizar **Driver**.
6. Selecione **Pesquisar automaticamente para atualizar o software do driver** e siga as instruções de instalação.