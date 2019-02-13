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
<span data-ttu-id="93f51-103">Se você estiver recebendo um erro durante a ativação do Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere a ativação ADAL editando o registro.</span><span class="sxs-lookup"><span data-stu-id="93f51-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="93f51-104">**Chave do Registro**</span><span class="sxs-lookup"><span data-stu-id="93f51-104">**Registry key**</span></span>|<span data-ttu-id="93f51-105">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="93f51-105">**Type**</span></span>|<span data-ttu-id="93f51-106">**Valor**</span><span class="sxs-lookup"><span data-stu-id="93f51-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="93f51-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="93f51-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="93f51-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="93f51-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="93f51-109">1</span><span class="sxs-lookup"><span data-stu-id="93f51-109">1</span></span>  <br/> |
   
<span data-ttu-id="93f51-110">Para obter mais informações, consulte [Ativar autenticação moderna do Office 2013 em dispositivos do Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="93f51-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="93f51-p101">ADAL é habilitado por padrão no Office 365 ProPlus e Office 2016. gt _ remote Desktop Services (RDS) era chamado de serviços de Terminal.</span><span class="sxs-lookup"><span data-stu-id="93f51-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

