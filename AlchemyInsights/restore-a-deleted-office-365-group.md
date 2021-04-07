---
title: Restaurar um grupo excluído do Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597431"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurar um grupo excluído do Microsoft 365

Você pode restaurar um grupo excluído do Microsoft 365 ou o Microsoft Teams dentro de 30 dias a partir da exclusão.

1. Vá para o Centro de administração do [Microsoft 365](https://aka.ms/RestoreDeletedGroup) para fazer logoff e listar os grupos e equipes excluídos.

    **Observação:** Faça logoff usando a conta atribuída ao administrador do locatário ou à função de administrador de grupos.

1. Selecione o grupo/Teams excluído do Microsoft 365 a ser restaurado e clique em **restaurar o grupo**.

    Se o grupo não puder ser restaurado devido a um endereço SMTP conflitante, use o seguinte comando para encontrar o objeto que está causando conflito e remover o endereço SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Observação:** Em alguns casos, pode levar até 24 horas para que o grupo e todos os seus dados sejam restaurados.

    Para obter mais informações ou saber como restaurar grupos usando o PowerShell, consulte [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).