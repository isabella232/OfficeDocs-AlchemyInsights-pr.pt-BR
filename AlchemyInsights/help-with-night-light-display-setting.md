---
title: Ajuda com a configuração de luz noturna
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
- "9005578"
- "9930"
ms.openlocfilehash: 7da8d4cefe2140340892544d73b9f8e3f3fdc679e9d58f2ad5ac12bf30830c5c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54078702"
---
# <a name="help-with-the-night-light-display-setting"></a>Ajuda com a configuração de luz noturna

Para saber mais sobre as configurações de exibição noturna, consulte [Agendar a exibição noturna no Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Se as opções de luz noturna estiverem desativadas em Configurações, verifique o driver de vídeo: 

1. Clique na caixa de pesquisa na barra de tarefas e digite **Gerenciador de Dispositivos** e selecione **Gerenciador de Dispositivos** nos resultados da pesquisa.
1. Expanda **adaptadores de vídeo**. 

Infelizmente, o recurso de luz noturna não estará disponível se o seu dispositivo usar um driver DisplayLink ou Basic Display.

O recurso de luz noturna usa tecnologia gráfica recente, portanto, pode ser necessário atualizar o driver de vídeo:  

- Verifique se há atualizações em **Iniciar** > **Configurações** > **Atualização e Segurança** > **Windows Update** > **Verificar se há atualizações**.  

OU

- Visite o site de suporte do fabricante de hardware para baixar e instalar manualmente os drivers de vídeo mais recentes.

## <a name="reset-night-light-in-the-registry"></a>Redefinir o modo de luz noturna no registro

Se a atualização do driver de vídeo não funcionar, pode ser necessário redefinir o modo de luz noturna no registro.  

**Cuidado:** esta etapa da solução de problemas é recomendada apenas para usuários avançados. Problemas graves podem ocorrer se você modificar o registro incorretamente. Para ter mais proteção, faça backup do registro antes de modificá-lo para que possa restaurá-lo se ocorrerem problemas.

1. Na caixa de pesquisa, digite **regedit** e selecione **Editor do Registro** nos resultados da pesquisa.

1. Vá para a seguinte chave de registro: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Exporte e exclua a seguinte subchave:$$windows.data.bluelightreduction.bluelightreductionstate

1. Exporte e exclua a seguinte subchave:$$windows.data.bluelightreduction.settings

1. Reinicie o Windows e verifique se as opções de luz noturna estão disponíveis.


