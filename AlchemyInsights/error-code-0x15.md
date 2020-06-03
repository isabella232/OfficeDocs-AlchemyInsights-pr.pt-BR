---
title: Código de erro 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se você estiver recebendo um erro ao ativar o Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere habilitar a ADAL editando o registro.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506834"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="567c1-103">Erro ao ativar o Office 2013 nos serviços de área de trabalho remota</span><span class="sxs-lookup"><span data-stu-id="567c1-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="567c1-104">Se você estiver recebendo um erro ao ativar o Office 2013 em implantações de serviços de área de trabalho remota (RDS), considere habilitar a ADAL editando o registro.</span><span class="sxs-lookup"><span data-stu-id="567c1-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="567c1-105">**Chave do Registro**</span><span class="sxs-lookup"><span data-stu-id="567c1-105">**Registry key**</span></span>|<span data-ttu-id="567c1-106">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="567c1-106">**Type**</span></span>|<span data-ttu-id="567c1-107">**Valor**</span><span class="sxs-lookup"><span data-stu-id="567c1-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="567c1-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="567c1-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="567c1-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="567c1-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="567c1-110">1 </span><span class="sxs-lookup"><span data-stu-id="567c1-110">1</span></span>  <br/> |

<span data-ttu-id="567c1-111">Para obter mais informações, consulte [habilitar a autenticação moderna do Office 2013 em dispositivos Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="567c1-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="567c1-112">A ADAL é habilitada por padrão no Microsoft 365 Apps for Enterprise e no Office 2016.</span><span class="sxs-lookup"><span data-stu-id="567c1-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="567c1-113">Os serviços de área de trabalho remota (RDS) eram chamados anteriormente dos serviços de terminal.</span><span class="sxs-lookup"><span data-stu-id="567c1-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  