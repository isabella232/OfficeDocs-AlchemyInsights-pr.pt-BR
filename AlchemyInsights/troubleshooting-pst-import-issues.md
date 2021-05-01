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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059803"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="1326f-102">Solucionar problemas de importação de PST</span><span class="sxs-lookup"><span data-stu-id="1326f-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="1326f-103">Se você estiver importando dentro do próprio cliente Outlook, confira [Corrigir problemas ao importar um arquivo .pst do Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="1326f-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="1326f-104">Se você estiver usando o Serviço de Importação e ele travar, observe que cada arquivo PST que você carrega no local de Armazenamento do Microsoft Azure não deve ser maior que 20 GB.</span><span class="sxs-lookup"><span data-stu-id="1326f-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="1326f-105">Arquivos PST com mais de 20 GB podem afetar o desempenho do processo de importação de PST.</span><span class="sxs-lookup"><span data-stu-id="1326f-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="1326f-106">Para obter mais informações sobre solução de problemas em trabalhos travados, confira [Problemas que afetam trabalhos de importação PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="1326f-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="1326f-107">Se você deseja verificar o status de um trabalho de importação específico, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="1326f-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="1326f-108">Para obter detalhes completos sobre o serviço de importação, confira [Visão geral da importação de arquivos PST da sua organização](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="1326f-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
