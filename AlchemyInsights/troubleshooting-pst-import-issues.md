---
title: Solucionar problemas de importação de PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991088"
---
# <a name="troubleshooting-pst-import-issues"></a>Solucionar problemas de importação de PST

- Se você estiver importando no próprio cliente do Outlook, confira [Corrigir problemas ao importar um arquivo .pst do Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Se você estiver usando o Serviço de Importação e ele estiver travado, observe que os arquivos PST carregados no local do Armazenamento do Azure não devem ultrapassar 20 GB. Os arquivos PST com mais de 20 GB podem afetar o desempenho do processo de importação de PST.

- Se você quiser verificar o status de um trabalho de Importação específico, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Para obter detalhes completos sobre o serviço de importação, confira [Visão geral sobre como importar arquivos PST da sua organização](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
