---
title: Implantação do aplicativo Win32 do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: d169dc0dd4e3cd9d94681d7db16ce3051677b708df02d3c9bd461855daabb295
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925873"
---
# <a name="intune-win32-app-deployment"></a>Implantação do aplicativo Win32 do Intune

O Microsoft Intune permite aplicativos Win32, incluindo, mas não se limitando a MSI, e .EXE para ser implantado em dispositivos Windows 10. O mecanismo de implantação usado exige que a extensão de gerenciamento do Intune (IME) esteja presente no dispositivo de destino. O IME será instalado automaticamente como resultado da implantação de um script do PowerShell ou do aplicativo Win32 em um usuário/dispositivo.

Há também um conjunto de pré-requisitos que devem ser atendidos para a implantação de aplicativos Win32 que incluem:

- Plataformas suportadas: Windows 10 versão 1607 ou posterior (versões Enterprise, Pro e Education).
- Arquiteturas suportadas: x86 e x64.
- Gerenciamento de dispositivo: o AAD ingressou e se registrou automaticamente (incluindo a política de grupo e de domínios híbridos).
- Formato de pacote de aplicativo: o arquivo **intunewin** preparado pela [ferramenta de preparação de conteúdo Win32 da Microsoft](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Limitações:
    - Tamanho máximo: 8 GB.
    - Arquitetura sem suporte: ARMs.

Examine o documento "[Adicionar, atribuir e monitorar um aplicativo Win32 no Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" para saber mais sobre essas etapas.

Detalhes de solução de problemas de implantação de aplicativos no Windows, incluindo aplicativos Win32, podem ser analisados nos seguintes documentos

- [Solucionar problemas de instalação do aplicativo](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Solucionar problemas de aplicativos Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)