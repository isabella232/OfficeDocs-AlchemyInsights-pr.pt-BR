---
title: Reparar arquivo. pst antes de importar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799084"
---
# <a name="repair-pst-file-before-importing"></a>Reparar arquivo. pst antes de importar

Antes de importar um arquivo. pst no Outlook, verifique se o arquivo não está corrompido reparando o arquivo:

1. Saia do Outlook.

2. Localize e execute `Scanpst.exe` na pasta de programa do Office (c:\Arquivos de programas (x86) \Microsoft Office\root\Office \<Version\> ou C:\Arquivos de Programas\Microsoft Office\root\Office \<Version\> ).

3. Na **ferramenta de reparo da caixa de entrada do Microsoft Outlook**, clique em **procurar** para localizar o arquivo. pst (por exemplo, em C:\Users \\<username \> \AppData\Local\Microsoft\Outlook). Selecione o arquivo. pst e clique em **abrir**.

4. Clique em **Iniciar** para iniciar a verificação.

5. Se forem encontrados erros no arquivo, clique em **reparar**e, em seguida, clique em **OK** quando o reparo estiver concluído.

6. Tente importar o arquivo. pst no Outlook novamente.

Para obter mais informações, consulte [reparar arquivos de dados do Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) e [corrigir problemas de importação de um arquivo. pst do Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
