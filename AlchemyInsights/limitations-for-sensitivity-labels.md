---
title: Limitações para rótulos de confidencialidade para arquivos do Office no SharePoint e no OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: 376c0293c325a725c117d54bb0f15b0146b9224c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332805"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Limitações para rótulos de confidencialidade para arquivos do Office no SharePoint e no OneDrive

Ao habilitar rótulos de confidencialidade para arquivos do Office no SharePoint e no OneDrive, esteja ciente dos requisitos e limitações, que incluem:

- O SharePoint e o OneDrive não podem processar alguns arquivos rotulados e criptografados de aplicativos da área de trabalho do Office quando os arquivos contêm dados do PowerQuery, dados armazenados por suplementos personalizados ou partes XML personalizadas.
- O SharePoint e o OneDrive não aplicam rótulos de confidencialidade automaticamente aos arquivos existentes que você já criptografou usando os rótulos Proteção de Informações do Azure (AIP). Para aplicar os rótulos de confidencialidade a arquivos criptografados: 
    - Verifique se os rótulos da AIP foram migrados e publicados no Centro de conformidade do Microsoft 365.
    - Baixe os arquivos rotulados e carregue-os no local original do SharePoint ou do OneDrive.
- Para documentos criptografados, não há suporte para impressão.

Para obter detalhes adicionais sobre limitações, consulte [Habilitar rótulos de confidencialidade para arquivos do Office no SharePoint e no OneDrive](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
