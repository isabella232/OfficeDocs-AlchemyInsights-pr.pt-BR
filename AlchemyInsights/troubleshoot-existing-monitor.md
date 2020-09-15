---
title: Solucionando problemas de monitor existente
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690699"
---
# <a name="troubleshoot-an-existing-monitor"></a>Solucionar problemas de um monitor existente

Experimente estas soluções para solucionar problemas de um monitor. 

**Atualize a exibição do seu monitor:**

Pressione as teclas a seguir ao mesmo tempo: tecla Windows + Ctrl + Shift + B. Isso atualizará a comunicação com seu driver de gráfico. Seus monitores piscarão momentaneamente e voltarão após alguns segundos.

**Solucionar problemas de hardware do monitor:**

1. Desconecte o cabo que conecta o computador ao monitor e conecte-o novamente.
2. Desconecte qualquer dispositivo não essencial do seu computador (como adaptadores ou cais).

**Se você instalou recentemente uma atualização no computador, pode reverter o seu driver de vídeo:**

1. Selecione **Iniciar**, digite **Gerenciador de dispositivos**e selecione **Gerenciador de dispositivos** nos resultados.
2. Expanda a seção **adaptadores de vídeo** , clique com o botão direito do mouse no adaptador de vídeo, es selecione **Propriedades**.
3. Navegue até a guia **Driver** e selecione **Reverter driver**. <br>
Observação: se isso não estiver disponível ou estiver esmaecido, selecione **não** nas opções abaixo para mover para a próxima etapa.
4. Talvez seja necessário reiniciar o computador para que as alterações entrem em vigor.

**Desinstalar e reinstalar o driver de vídeo:**

1. Selecione **Iniciar**, digite **Gerenciador de dispositivos**e selecione **Gerenciador de dispositivos** nos resultados.
2. Expanda a seção **adaptadores de vídeo** , clique com o botão direito do mouse no adaptador de vídeo, es selecione **desinstalar dispositivo**. 
3. Selecione a caixa ao lado de **excluir o software de driver para este dispositivo** e selecione **desinstalar**.<br>
Observação: você pode ser solicitado a reiniciar o computador neste estágio. Certifique-se de anotar as instruções restantes antes de reiniciar.
4. Abra o Gerenciador de dispositivos novamente.
5. Expanda a seção **adaptadores de vídeo** , clique com o botão direito do mouse no adaptador de vídeo e selecione **Atualizar driver**.
6. Selecione **Pesquisar automaticamente o software de driver de atualização** e siga as instruções de instalação.