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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972407"
---
# <a name="troubleshooting-pst-import-issues"></a>Solucionar problemas de importação de PST

- Se você estiver importando dentro do próprio cliente Outlook, confira [Corrigir problemas ao importar um arquivo .pst do Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Se você estiver usando o Serviço de Importação e ele travar, observe que cada arquivo PST que você carrega no local de Armazenamento do Microsoft Azure não deve ser maior que 20 GB. Arquivos PST com mais de 20 GB podem afetar o desempenho do processo de importação de PST. Para obter mais informações sobre solução de problemas em trabalhos travados, confira [Problemas que afetam trabalhos de importação PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Se você deseja verificar o status de um trabalho de importação específico, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Para obter detalhes completos sobre o serviço de importação, confira [Visão geral da importação de arquivos PST da sua organização](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
