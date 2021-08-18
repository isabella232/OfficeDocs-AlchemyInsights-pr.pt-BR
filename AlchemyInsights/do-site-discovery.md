---
title: Fazer descoberta do site
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
- "9143"
- "9005291"
ms.openlocfilehash: 5ae99192c769dd5d5acae1c6e8f9b021e824b465
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322155"
---
# <a name="do-site-discovery"></a>Fazer descoberta do site

Se a sua organização ainda usa aplicativos da web legados e planeja usar o modo Internet Explorer (o que a maioria dos clientes faz), você deve fazer algumas descobertas de sites adicionais.

**Você já implantou uma versão mais antiga do Microsoft Edge**

Se você já configurou sua Lista de Sites da Empresa para funcionar com a versão herdada do Microsoft Edge, a descoberta de seu site está quase concluída. A única coisa que você precisa fazer é adicionar sites neutros.

Sites neutros são normalmente sites que fornecem logon único (SSO). Se você for a um site neutro do Microsoft Edge, deseja permanecer no Microsoft Edge para fazer a autenticação. Se você for para um site neutro no modo Internet Explorer, deverá permanecer no modo Internet Explorer para fazer a autenticação.

Identifique qualquer SSO ou outros sites neutros que você usa e adicione-os à sua Lista de Sites da Empresa.

**Internet Explorer é o seu navegador padrão**

Se você estiver usando apenas o Internet Explorer agora, talvez não saiba quais sites foram atualizados para os padrões modernos da web e quais ainda exigem o Internet Explorer. Você desejará localizar e adicionar esses sites à Lista de Sites da Empresa para que possa usar o modo Internet Explorer apenas para esses sites.

**Observação**: [Descoberta de Sites da Empresa](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) descobre sites que podem precisar do modo Internet Explorer. Ele pode coletar dados em computadores que executam o Windows Internet Explorer 8 por meio do Internet Explorer 11 no Windows 10, Windows 8.1 ou Windows 7.

**Analisar os dados**

Depois de coletar os dados do site, recomendamos o seguinte processo de quatro etapas para analisar os dados:
1. Classifique os dados por domínio e, em seguida, por URL.
2. Defina os limites de um aplicativo a ser configurado para o modo Internet Explorer. Você deseja incluir todos os sites e controles da web que definem o aplicativo, mas não deseja incluir sites e controles extras. Alguns sites podem ser tão simples como o *https://contoso.com/app1* enquanto outros podem exigir que você defina vários sites e páginas.
3. Teste o aplicativo para verificar se ele não funciona nativamente. Muitos sites oferecerão conteúdo moderno quando detectarem um navegador moderno e só oferecerão conteúdo herdado quando detectarem Internet Explorer.
4. Adicione o aplicativo à sua Lista de Sites de Empresas se ele falhar no teste.

**Observação**: Como prática recomendada, agrupe todos os sites que compõem um aplicativo. Dessa forma, quando você atualiza um aplicativo, é mais fácil remover todo o site do modo Internet Explorer e começar a usar um navegador moderno para esse aplicativo.

Depois de concluir a descoberta do site e analisar os dados, você está pronto para começar a analisar sua estratégia de canal.

