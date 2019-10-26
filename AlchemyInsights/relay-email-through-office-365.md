---
title: Retransmitir emails no Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: e971593b7a67e1bb40243fc762bace6b87a35741
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745385"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="16e56-102">Configurar um dispositivo multifuncional ou aplicativo para enviar email usando o Office 365</span><span class="sxs-lookup"><span data-stu-id="16e56-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="16e56-103">Saiba mais sobre as opções e etapas necessárias em [Como configurar um dispositivo ou aplicativo multifuncional para enviar emails usando o Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="16e56-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="16e56-104">**Observação:** se você tiver um dispositivo ou aplicativo que parou recentemente de funcionar, observe que recentemente [desativamos a codificação 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) conforme havia sido planejado.</span><span class="sxs-lookup"><span data-stu-id="16e56-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="16e56-105">Para ver os dispositivos afetados, vá para o [Relatório de clientes de Autenticação SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="16e56-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="16e56-106">Os erros comuns podem ser: falha/erro de autenticação, falha/erro de TLS, erro de algoritmo de codificação, incompatibilidade de algoritmo ou conexão interrompida.</span><span class="sxs-lookup"><span data-stu-id="16e56-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="16e56-107">Para resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="16e56-107">To resolve this issue:</span></span>
 - <span data-ttu-id="16e56-108">**O SMTP do IIS do Windows Server 2003 deixará de funcionar. É necessária uma versão mais recente do Windows.**</span><span class="sxs-lookup"><span data-stu-id="16e56-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="16e56-109">Entre em contato com o fornecedor do aplicativo ou do dispositivo para verificar se há uma atualização ou uma criptografia moderna compatível.</span><span class="sxs-lookup"><span data-stu-id="16e56-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
