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
ms.openlocfilehash: 22430e2b8a00023f9922fd59d6fcabd308d08453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317220"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testar a Configuração do IRM para novas funcionalidades do OME

Para verificar se o locatário do Microsoft 365 está configurado para usar os novos recursos OME, execute os seguintes cmdlets enquanto estiver conectado ao [PowerShell do Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell):


1. Verifique a configuração do IRM do locatário executando `Get-IRMConfiguration`. Verifique se esses valores estão definidos como **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Usando seu domínio, endereço do remetente e destinatário, execute `Test-IRMConfiguration`. Se o teste não for aprovado, investigue sua configuração de IRM.

Para obter mais informações sobre como verificar a configuração do IRM, consulte [Verificar a nova configuração do OME no PowerShell do Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).