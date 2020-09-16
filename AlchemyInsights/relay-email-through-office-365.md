---
title: Retransmitir emails no Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 180bae451941e4aaea94d285362794a797383eca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776474"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="b7720-102">Configurar um dispositivo multifuncional ou aplicativo para enviar email</span><span class="sxs-lookup"><span data-stu-id="b7720-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="b7720-103">Saiba mais sobre as opções e etapas necessárias em [Como configurar um dispositivo ou aplicativo multifuncional para enviar emails usando o Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="b7720-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="b7720-104">**Observação:** se você tiver um dispositivo ou aplicativo que parou recentemente de funcionar, observe que recentemente [desativamos a codificação 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) conforme havia sido planejado.</span><span class="sxs-lookup"><span data-stu-id="b7720-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="b7720-105">Para ver os dispositivos afetados, vá para o [Relatório de clientes de Autenticação SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b7720-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="b7720-106">Os erros comuns podem ser: falha/erro de autenticação, falha/erro de TLS, erro de algoritmo de codificação, incompatibilidade de algoritmo ou conexão interrompida.</span><span class="sxs-lookup"><span data-stu-id="b7720-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="b7720-107">Para resolver o problema:</span><span class="sxs-lookup"><span data-stu-id="b7720-107">To resolve the issue:</span></span>

 - <span data-ttu-id="b7720-108">**O SMTP do IIS do Windows Server 2003 deixará de funcionar. É necessária uma versão mais recente do Windows.**</span><span class="sxs-lookup"><span data-stu-id="b7720-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="b7720-109">Entre em contato com o fornecedor do aplicativo ou do dispositivo para verificar se há uma atualização ou uma criptografia moderna compatível.</span><span class="sxs-lookup"><span data-stu-id="b7720-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
