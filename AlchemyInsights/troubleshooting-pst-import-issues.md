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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="5809b-102">Solucionar problemas de importação de PST</span><span class="sxs-lookup"><span data-stu-id="5809b-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="5809b-103">Se você estiver importando no próprio cliente do Outlook, confira [Corrigir problemas ao importar um arquivo .pst do Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="5809b-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="5809b-104">Se você estiver usando o Serviço de Importação e ele estiver travado, observe que os arquivos PST carregados no local do Armazenamento do Azure não devem ultrapassar 20 GB.</span><span class="sxs-lookup"><span data-stu-id="5809b-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="5809b-105">Os arquivos PST com mais de 20 GB podem afetar o desempenho do processo de importação de PST.</span><span class="sxs-lookup"><span data-stu-id="5809b-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="5809b-106">Se você quiser verificar o status de um trabalho de Importação específico, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="5809b-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="5809b-107">Para obter detalhes completos sobre o serviço de importação, confira [Visão geral sobre como importar arquivos PST da sua organização](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="5809b-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
