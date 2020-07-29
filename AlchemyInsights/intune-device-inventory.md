---
title: Inventário de dispositivos do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434567"
---
# <a name="intune-device-inventory"></a>Inventário de dispositivos do Intune

A lâmina de Dispositivos fornece ao administrador uma visão geral dos dispositivos em gerenciamento do Intune por dispositivo. As informações mostradas incluem: hardware, aplicativos descobertos, estado de conformidade de dispositivos e estado de configuração do dispositivo.

Os dados de inventário para hardware e aplicativos descobertos são coletados em um ciclo de sete dias. Os aplicativos e os elementos específicos do hardware relatado são diferentes dependendo do sistema operacional do dispositivo e se o dispositivo é pessoal ou corporativo.

Para obter mais informações, confira [Ver detalhes do dispositivo no Intune](https://docs.microsoft.com/intune/device-inventory).

**Perguntas Frequentes**

P: Não estou recebendo uma lista completa de inventários dos aplicativos presentes nos dispositivos Windows registrados no Intune. Por que não?

R: No momento, somente os aplicativos modernos estão listados para PCs com Windows 10, identificados como dispositivos corporativos. O Intune não coletará informações sobre aplicativos Win32 instalados nesses dispositivos.

P: Por que os números de telefone não são coletados em todos os dispositivos?

R: Os telefones classificados como dispositivos corporativos no Intune não serão identificados com o número de telefone inteiro quando, por exemplo, você executar um relatório de inventário de dispositivo móvel. Os números de telefone de todos os dispositivos são sempre mascarados parcialmente por asteriscos (****) e mostram somente os últimos quatro dígitos.