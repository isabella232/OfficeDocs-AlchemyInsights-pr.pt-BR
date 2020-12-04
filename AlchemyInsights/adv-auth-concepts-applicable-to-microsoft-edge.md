---
title: Conceitos de autenticação avançada aplicáveis ao Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571764"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Conceitos de autenticação avançada aplicáveis ao Microsoft Edge

Veja a seguir os conceitos de autenticação avançada que se aplicam ao Microsoft Edge:

**Autenticação proativa**

Quando você habilita a política [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , o Microsoft Edge tenta autenticar proativamente usuários conectados através dos serviços da Microsoft. Em intervalos regulares, ele usará um serviço online para verificar se há um manifesto atualizado que contenha a configuração de controle de autenticação proativa.

Benefícios: a autenticação pró-ativa habilita a autenticação para os principais serviços, como a página de nova guia do Office. Além disso, se o Bing for usado como o mecanismo de pesquisa, a autenticação pró-ativa melhorará o desempenho da barra de endereços e ajudará a gerar resultados de pesquisa personalizados para as necessidades de sua empresa.

**Windows Hello CredUI para autenticação NTLM**

Se o logon único (SSO) não estiver disponível quando um site tentar entrar no usuário por meio do mecanismo NTLM ou Negotiate, este recurso permitirá que o usuário Compartilhe as credenciais do sistema operacional com o site e satisfaça o desafio de autenticação usando a IU de credenciais do Windows Hello. Esse fluxo de logon aparecerá apenas no Windows 10 e apenas para usuários que não obtêm SSO durante um Challenge NTLM ou negociar.

**Usar senhas salvas para entrar automaticamente**

Os usuários que salvam senhas no Microsoft Edge podem habilitar o logon automático para sites onde foram salvas credenciais. Os usuários podem ativar ou desativar esse recurso no edge://settings/passwords, e você pode configurá-lo nas políticas do [Gerenciador de senhas](https://go.microsoft.com/fwlink/?linkid=2134622) .
