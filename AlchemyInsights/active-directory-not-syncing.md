---
title: Não sincronização do Active Directory
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314192"
---
# <a name="active-directory-not-syncing"></a>Não sincronização do Active Directory

Se você estiver recebendo erros de sincronização, como "nenhuma sincronização recente", ou observe que o status de sincronização de diretório no portal de administração do Office diz: "A última sincronização foi há mais de 3 dias", pode ser que o AADConnect tenha configurações incorretas ou permissões insuficientes para executar uma sincronização.  

Reinstalar o AADConnect usando configurações expressas pode resolver o problema rapidamente:

1. [Baixe a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Siga as instruções para instalação expressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

O Azure AD Connect deve ser instalado no Windows Server 2012 ou versão mais recente. Esse servidor deve ser integrado ao domínio e pode ser um controlador de domínio ou um servidor membro. Para uma lista completa de requisitos e pré-requisitos do Azure AD Conexão, revise Os pré-requisitos do [Azure AD Conexão](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Para mais informações sobre contas de serviço do AADConnect, confira [Azure AD Connect: Contas e permissões](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
