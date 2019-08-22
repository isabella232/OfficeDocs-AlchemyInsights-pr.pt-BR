---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se você estiver recebendo um erro ao ativar o Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere habilitar a ADAL editando o registro.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526959"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Erro ao ativar o Office 2013 nos serviços de área de trabalho remota

Se você estiver recebendo um erro ao ativar o Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere habilitar a ADAL editando o registro.
  
|**Chave do Registro**|**Tipo**|**Valor**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Para obter mais informações, consulte [habilitar a autenticação moderna do Office 2013 em dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  A ADAL está habilitada por padrão no Office 365 ProPlus e no Office 2016. Os serviços de área de trabalho remota (RDS) eram chamados anteriormente dos serviços de terminal.
  