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
ms.openlocfilehash: 1f286896f80a6bbabd4810f10fb0b8284fd13aba
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58311351"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Envio de unidade no Serviço de Importação do Microsoft 365

Use o Envio de unidade copiando PSTs para um disco rígido e envie-o para a Microsoft.

Para iniciar o trabalho:

1. No Centro de Conformidade do Microsoft 365, em **Governança de Informações**, selecione **Importar**.

1. Selecione **Escolher tipo de trabalho de importação** e depois selecione **Avançar**.

1. Para ver as etapas para esta opção de importação, selecione **Enviar riscos rígido para um de nossos locais físicos**.

Aqui estão algumas coisas importantes a serem lembradas:

- Você deverá ter a função Exportação de Importação de Caixa de Correio no Exchange Online para importar arquivos PST para as caixas de correio do Microsoft 365. O desempenho pode ser afetado para PSTs maiores que 20 GB.

- Somente as unidades de estado sólido (SSDs) de 2,5 polegadas ou discos rígidos internos SATA II/III de 2,5 ou 3,5 polegadas são compatíveis.
O disco rígido contendo os arquivos PST deve ser criptografado com BitLocker.

- O custo de importação dos arquivos PST para as caixas de correio do Microsoft 365 usando o envio de unidade é de US$ 2 por GB de dados.

Para obter mais informações sobre o uso do método de envio de unidade para importação de PSTs, veja [Usar envio de unidade para importar os arquivos PST da sua organização](https://docs.microsoft.com/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).