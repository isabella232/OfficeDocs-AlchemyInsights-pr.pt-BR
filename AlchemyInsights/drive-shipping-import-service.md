---
title: Envio de unidade no Serviço de Importação do Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721661"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="66143-102">Envio de unidade no Serviço de Importação do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="66143-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="66143-103">Use o Envio de unidade copiando PSTs para um disco rígido e envie-o para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="66143-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="66143-104">Para iniciar o trabalho:</span><span class="sxs-lookup"><span data-stu-id="66143-104">To start the job:</span></span>

1. <span data-ttu-id="66143-105">No Centro de Conformidade do Microsoft 365, em **Governança de Informações**, selecione **Importar**.</span><span class="sxs-lookup"><span data-stu-id="66143-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="66143-106">Selecione **Escolher tipo de trabalho de importação** e depois selecione **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="66143-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="66143-107">Para ver as etapas para esta opção de importação, selecione **Enviar riscos rígido para um de nossos locais físicos**.</span><span class="sxs-lookup"><span data-stu-id="66143-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="66143-108">Aqui estão algumas coisas importantes a serem lembradas:</span><span class="sxs-lookup"><span data-stu-id="66143-108">Here are some things to remember:</span></span>

- <span data-ttu-id="66143-109">Você deverá ter a função Exportação Importação da Caixa de Correio no Exchange Online para importar arquivos PST para as caixas de correio do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="66143-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="66143-110">O desempenho pode ser afetado para PSTs maiores que 20Gb.</span><span class="sxs-lookup"><span data-stu-id="66143-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="66143-111">Somente as unidades de estado sólido (SSDs) de 2,5 polegadas ou discos rígidos internos SATA II/III de 2,5 ou 3,5 polegadas são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="66143-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="66143-112">O disco rígido contendo os arquivos PST deve ser criptografado com BitLocker.</span><span class="sxs-lookup"><span data-stu-id="66143-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="66143-113">O custo de importação dos arquivos PST para as caixas de correio do Microsoft 365 usando o envio de unidade é de US$ 2 por GB de dados.</span><span class="sxs-lookup"><span data-stu-id="66143-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="66143-114">Para obter mais informações sobre o uso do método de envio de unidade para importação de PSTs, veja [Usar envio de unidade para importar os arquivos PST da sua organização](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span><span class="sxs-lookup"><span data-stu-id="66143-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>