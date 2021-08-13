---
title: Registros de senha
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960931"
---
# <a name="password-logs"></a>Registros de senha

**Estou tendo problemas para acessar os registros de auditoria de redefinição de senha**

Para solucionar problemas relacionados ao acesso aos logs de auditoria de redefinição de senha, execute a seguinte etapa:

Certifique-se de que você está autorizado a visualizar os logs de auditoria. 

Apenas as seguintes funções são autorizadas:
 - Administrador global
 - Administrador de segurança
 - Leitor de segurança

**Quero ver todos os eventos de auditoria de redefinição de senha desde o momento inicial em que foi implantado**

Até 120.000 eventos de redefinição/registro de senha são armazenados nos relatórios dos últimos 30 dias. Este limite máximo se aplica à IU quando estiver baixando o CSV. 1 milhão de eventos estão disponíveis por meio do Windows PowerShell.
Para obter mais informações, consulte os links abaixo:

- [Eventos de autoatendimento de redefinição de senha a partit da API de Relatórios e Eventos do Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Como baixar eventos de registro de redefinição de senha rapidamente com o Windows PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Quero entender mais sobre os recursos de relatório de redefinição de senha**

Verifique quem está se registrando ou redefinindo senhas com logs de auditoria de redefinição de senha do Microsoft Azure Active Directory no portal do Azure em **Usuários e grupos**.
Para obter mais informações, consulte os seguintes links:

- [Visão geral dos relatórios de redefinição de senha](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Como visualizar os relatórios de redefinição de senha no portal do Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Eventos de autoatendimento de redefinição de senha a partit da API de Relatórios e Eventos do Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Como baixar eventos de registro de redefinição de senha rapidamente com o Windows PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


