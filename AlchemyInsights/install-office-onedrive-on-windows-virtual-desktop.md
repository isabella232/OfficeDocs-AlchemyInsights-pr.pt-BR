---
title: Instalar o Office e o OneDrive na Área de Trabalho Virtual do Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590258"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instalar o Office e o OneDrive na Área de Trabalho Virtual do Windows

1. [Preparar e personalizar uma imagem VHD mestra](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Crie uma máquina virtual (VM), caso ainda não tenha sido criada.

1. [Instale o Office no modo de ativação de computador compartilhado](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). A ativação de computador compartilhado permite que vários usuários acessem o Office.

1. [Instale o OneDrive no modo por máquina](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Normalmente, o OneDrive é instalado por usuário, mas aqui ele deve ser instalado por máquina.