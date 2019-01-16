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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274781"
---
<span data-ttu-id="2f392-103">Se você estiver recebendo um erro durante a ativação do Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere a ativação ADAL editando o registro.</span><span class="sxs-lookup"><span data-stu-id="2f392-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="2f392-104">**Chave do Registro**</span><span class="sxs-lookup"><span data-stu-id="2f392-104">**Registry key**</span></span>|<span data-ttu-id="2f392-105">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="2f392-105">**Type**</span></span>|<span data-ttu-id="2f392-106">**Valor**</span><span class="sxs-lookup"><span data-stu-id="2f392-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2f392-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="2f392-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="2f392-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="2f392-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="2f392-109">1</span><span class="sxs-lookup"><span data-stu-id="2f392-109">1</span></span>  <br/> |
   
<span data-ttu-id="2f392-110">Para obter mais informações, consulte [Ativar autenticação moderna do Office 2013 em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="2f392-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="2f392-p101">ADAL é habilitado por padrão no Office 365 ProPlus e Office 2016. > Serviços de área de trabalho remota (RDS) era chamado de serviços de Terminal.</span><span class="sxs-lookup"><span data-stu-id="2f392-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

