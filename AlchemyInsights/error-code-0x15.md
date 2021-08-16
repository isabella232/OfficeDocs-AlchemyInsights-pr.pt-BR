---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se você estiver recebendo um erro ao ativar o Office 2013 em implantações de Serviços de Área de Trabalho Remota (RDS), considere habilitar o ADAL editando o Registro.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100750"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Erro durante a ativação Office 2013 nos Serviços de Área de Trabalho Remota

Se você estiver recebendo um erro ao ativar o Office 2013 em implantações de Serviços de Área de Trabalho Remota (RDS), considere habilitar o ADAL editando o Registro.
  
|**Chave do Registro**|**Tipo**|**Valor**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Para obter mais informações, consulte [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  O ADAL é habilitado por padrão no Microsoft 365 Apps para Grandes Empresas e Office 2016. O RDS (Serviços de Área de Trabalho Remota) foi anteriormente chamado de Serviços de Terminal.
  