---
title: Instalar o servidor de relatório do Power BI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 3ea596547093773ab872ca34e8dd3a4e49e59fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755083"
---
# <a name="install-power-bi-report-server"></a>Instalar o servidor de relatório do Power BI

1. Encontre o local de PowerBIReportServer.exe e inicie o instalador.

2. Selecione **instalar o servidor de relatório do Power bi**.

3. Escolha uma edição para instalar e, em seguida, selecione **Avançar**.

4. Você pode escolher Evaluation ou Developer Edition no menu suspenso.  Caso contrário, você pode inserir uma chave do produto (Product Key) para o servidor adquirido do serviço do Power BI ou do centro de serviços de licenciamento por volume. Para obter mais informações sobre como obter sua chave do produto, consulte a seção antes de começar. Leia e concorde com os termos e condições da licença e selecione **Avançar**.

5. Você precisa ter um mecanismo de banco de dados disponível para armazenar o banco de dados do servidor de relatório. Selecione **Avançar** para instalar somente o servidor de relatório.

6. Especifique o local de instalação para o servidor de relatório. Selecione **instalar** para continuar.

7. Após uma instalação bem-sucedida, selecione **Configurar servidor de relatório** para iniciar o Gerenciador de configuração do Reporting Services.

Você não precisa de um servidor de mecanismo de banco de dados do SQL Server disponível no momento da instalação. Será necessário um para configurar o Reporting Services após a instalação.

Para obter mais informações: https://docs.microsoft.com/power-bi/report-server/install-report-server
