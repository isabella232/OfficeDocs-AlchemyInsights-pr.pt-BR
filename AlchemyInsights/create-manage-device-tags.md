---
title: Criar e gerenciar marcas ou grupos de dispositivo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 752d08ce7583580ac9896bd4390152df493d7148c8e8d4a1f39d86fc87785a7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069520"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Criar e gerenciar marcas ou grupos de dispositivo

Adicionar marcas em dispositivos para criar uma afiliação de grupo lógico. As marcas de dispositivo oferecem suporte ao mapeamento correto da rede, permitindo anexar marcas diferentes para capturar contexto e habilitar a criação de lista dinâmica como parte de um incidente. As marcas podem ser usadas como um filtro no modo de exibição de lista Dispositivos ou para agrupar dispositivos. Para obter mais informações sobre agrupamento de dispositivos, veja [Criar e gerenciar marcas de dispositivo](/microsoft-365/security/defender-endpoint/machine-tags).

Você pode adicionar marcas em dispositivos ao:

- Usar o portal

- Definir um valor de chave de registro
 
**Observação:** Pode haver latência entre o momento que uma marca for adicionada a um dispositivo e sua disponibilidade na lista de dispositivos e na página de dispositivo.

Para adicionar marcas de dispositivo usando a API, veja a [API Adicionar ou remover marcas de dispositivo](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).

## <a name="add-and-manage-device-tags-using-the-portal"></a>Adicionar e gerenciar marcas de dispositivo usando o portal

1. Selecione o dispositivo o qual você deseja gerenciar as marcas. Você pode selecionar ou procurar um dispositivo a partir de qualquer uma dos modos de exibição a seguir:

    - **Painel de operações de segurança** Selecione o nome do dispositivo nos Principais dispositivos com a seção de alertas ativos.
    - **Fila de alertas** - Selecione o nome do dispositivo ao lado do ícone do dispositivo na fila de alertas.
    - **Lista de dispositivos** - Selecione o nome do dispositivo na lista de dispositivos.
    - **Caixa de pesquisa** - Selecione Dispositivo no menu suspenso e insira o nome do dispositivo.

    Você também pode acessar a página de alertas através do modo de exibição de arquivo e IP.

1. Selecione **Gerenciar Marcas** na linha de ações de Resposta.

1. Digitar para localizar ou criar marcas.

As marcas são adicionadas ao modo de exibição do dispositivo e são refletidas no modo de exibição de lista Dispositivos. Depois, você poderá usar o filtro Marcas para ver a lista relevante de dispositivos.

Para saber mais, veja [Criar e gerenciar marcas de dispositivo](/microsoft-365/security/defender-endpoint/machine-tags).