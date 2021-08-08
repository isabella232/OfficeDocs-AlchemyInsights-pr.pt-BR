---
title: Testar a Configuração do IRM para novas funcionalidades do OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53908967"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testar a Configuração do IRM para novas funcionalidades do OME

Para verificar se o locatário do Microsoft 365 está configurado para usar os novos recursos OME, execute os seguintes cmdlets enquanto estiver conectado ao [PowerShell do Exchange Online](/powershell/exchange/exchange-online-powershell):


1. Verifique a configuração do IRM do locatário executando `Get-IRMConfiguration`. Verifique se esses valores estão definidos como **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Usando seu domínio, endereço do remetente e destinatário, execute `Test-IRMConfiguration`. Se o teste não for aprovado, investigue sua configuração de IRM.

Para obter mais informações sobre como verificar a configuração do IRM, consulte [Verificar a nova configuração do OME no PowerShell do Exchange Online](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).