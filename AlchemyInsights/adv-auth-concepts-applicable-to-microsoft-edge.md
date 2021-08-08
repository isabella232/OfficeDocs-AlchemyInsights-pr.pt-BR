---
title: Conceitos avançados de autenticação aplicáveis Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934353"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Conceitos avançados de autenticação aplicáveis Microsoft Edge

A seguir estão os conceitos avançados de autenticação aplicáveis a Microsoft Edge:

**Autenticação Proativa**

Quando você habilitar [a política ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge tentará autenticar proativamente os usuários in-lo serviços Microsoft. Em intervalos regulares, ele usará um serviço online para verificar se há um manifesto atualizado que contém a configuração que rege a Autenticação Proativa.

Benefícios: a Autenticação Proativa habilita a autenticação para serviços principais, como a Office Nova Guia. Além disso, se Bing for usado como mecanismo de pesquisa, a Autenticação Proativa melhora o desempenho da barra de endereços e ajuda a gerar resultados de pesquisa personalizados para as necessidades da sua empresa.

**Windows Hello CredUI para autenticação NTLM**

Se o SSO (login único) não estiver disponível quando um site tentar entrar no usuário por meio do mecanismo NTLM ou Negociar, esse recurso permitirá que o usuário compartilhe as credenciais do sistema operacional com o site e atenda ao desafio de autenticação usando a interface do usuário cred Windows Hello Cred. Esse fluxo de login aparecerá somente no Windows 10 e somente para usuários que não receberem SSO durante um NTLM ou um desafio Negociar.

**Usar senhas salvas para entrar automaticamente**

Os usuários que salvam senhas em Microsoft Edge podem habilitar o login automático em sites onde salvaram credenciais. Os usuários podem ativar ou desativar esse recurso edge://settings/passwords e você pode configurá-lo nas políticas de gerenciador [de](https://go.microsoft.com/fwlink/?linkid=2134622) senhas.
