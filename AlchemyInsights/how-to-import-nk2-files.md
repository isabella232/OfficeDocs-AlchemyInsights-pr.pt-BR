---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043194"
---
# <a name="how-to-import-nk2-files"></a>Como importar arquivos .nk2 

Quando você inicia Microsoft Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para Microsoft 365 pela primeira vez, seu cache de apelido (armazenado no arquivo .nk2 *profilename)* é importado para uma mensagem oculta no seu armazenamento de mensagens padrão.

Para importar arquivos .nk2 para o Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para Microsoft 365, certifique-se de que o arquivo .nk2 está na seguinte pasta: %appdata%\Microsoft\Outlook

**Observação**: o arquivo .nk2 deve ter o mesmo nome do seu perfil Outlook 2013 ou Outlook 2016 2013. Por padrão, o nome do perfil é "Outlook". Para verificar o nome do perfil, siga estas etapas: 
1. Clique em **Iniciar** e depois em **Painel de Controle**.
2. Clique duas vezes em **Email**.
3. Na caixa de diálogo Configuração de Email, selecione **Mostrar Perfis**.
4. Selecione **Iniciar** > **Executar**.
5. Na caixa **Abrir,** digite *outlook.exe /importnk2* e selecione **OK**. 

Depois de importar o arquivo .nk2, o conteúdo do arquivo será mesclado no cache de apelido existente armazenado em sua caixa de correio.

**Observação**: o arquivo .nk2 é renomeado com uma extensão de nome de arquivo .old na próxima vez que você iniciar Outlook 2013, Outlook 2016, Outlook 2019 ou Outlook para Microsoft 365. Se quiser importar o arquivo .nk2 de novo, remova primeiro a extensão de nome de arquivo .old.

Para obter mais informações, [consulte Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).