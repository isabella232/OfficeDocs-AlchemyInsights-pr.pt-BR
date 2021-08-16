---
title: Erro 4c7 do Teams
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
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049296"
---
# <a name="4c7-error-in-microsoft-teams"></a>Erro 4c7 no Microsoft Teams

Este erro ocorre porque o Microsoft Teams requer autenticação de formulários. Ao implantar o Serviços de Federação do Active Directory (AD FS), a Autenticação de Formulários não é habilitada para a intranet por padrão. Se a Autenticação Integrada do Windows falhar, você será solicitado a entrar usando Autenticação de Formulários.

Para resolver esse problema, habilite a Autenticação de Formulários usando o snap-in do MMC (Console de Gerenciamento Microsoft) do Serviços de Federação do Active Directory (AD FS) no computador que tem a cópia local do Active Directory. Para fazer isso, execute estas etapas: 

1. No painel de navegação, navegue até **Políticas de Autenticação**.
2. Em **Ações**, no painel detalhes, selecione **Edite a Autenticação Primária Global**.
3. Na guia **Intranet**, selecione **Autenticação de Formulários**.
4. Selecione **OK** (ou **Salvar**). 