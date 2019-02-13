---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se você estiver recebendo um erro durante a ativação do Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere a ativação ADAL editando o registro.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929076"
---
Se você estiver recebendo um erro durante a ativação do Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere a ativação ADAL editando o registro. 
  
|**Chave do Registro**|**Tipo**|**Valor**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Para obter mais informações, consulte [Ativar autenticação moderna do Office 2013 em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL é habilitado por padrão no Office 365 ProPlus e Office 2016. gt _ remote Desktop Services (RDS) era chamado de serviços de Terminal. 
  

