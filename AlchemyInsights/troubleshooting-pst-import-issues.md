---
title: Solucionar problemas de importação de PST
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
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826151"
---
# <a name="troubleshooting-pst-import-issues"></a>Solucionar problemas de importação de PST

- Se você estiver importando no próprio cliente do Outlook, confira [Corrigir problemas ao importar um arquivo .pst do Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Se você estiver usando o Serviço de Importação e ele estiver travado, observe que os arquivos PST carregados no local do Armazenamento do Azure não devem ultrapassar 20 GB. Os arquivos PST com mais de 20 GB podem afetar o desempenho do processo de importação de PST.

- Se você quiser verificar o status de um trabalho de Importação específico, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Para obter detalhes completos sobre o serviço de importação, confira [Visão geral sobre como importar arquivos PST da sua organização](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
