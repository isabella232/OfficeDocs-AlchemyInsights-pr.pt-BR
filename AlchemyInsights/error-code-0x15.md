---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se você estiver recebendo um erro durante a ativação do Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere a ativação ADAL editando o registro.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499370"
---
Se você estiver recebendo um erro durante a ativação do Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere a ativação ADAL editando o registro. 
  
|**Chave do Registro**|**Tipo**|**Valor**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |^1  <br/> |
   
Para obter mais informações, consulte [Ativar autenticação moderna do Office 2013 em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL é habilitado por padrão no Office 365 ProPlus e Office 2016. gt _ remote Desktop Services (RDS) era chamado de serviços de Terminal. 
  

