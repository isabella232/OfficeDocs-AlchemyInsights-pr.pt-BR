---
title: Usar o TeamViewer para administrar remotamente dispositivos do Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505174"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Usar o TeamViewer para administrar remotamente dispositivos do Intune

Os dispositivos gerenciados pelo Intune podem ser administrados remotamente usando [TeamViewer](https://www.teamviewer.com/).

Para administrar o Intune usando o TeamViewer, siga estas etapas: 

Comece obtendo as credenciais do TeamViewer para configurar o conector do TeamViewer no Intune. Isso permite que o administrador insira as credenciais na interface do usuário do conector do TeamViewer em dispositivos, uma operação única para estabelecer o vínculo entre o Intune e o serviço do TeamViewer.

**Parte 1: Iniciar uma sessão com um dispositivo remoto**

1. Em **Todos os dispositivos**, selecione o dispositivo com o qual você deseja iniciar uma sessão remota.
2. De **... Mais**, selecione **Nova sessão de assistência remota**.
3. Selecione **Sim** para confirmar que você deseja estabelecer uma sessão remota.
    Após a solicitação "Iniciando uma nova sessão remota" ser reconhecida pelo serviço TeamViewer, você verá uma opção para **Iniciar a assistência remota** em detalhes do painel Visão geral (ou, Essenciais) para o dispositivo. Selecione **Ver mais** para expandir o painel e mostrar o status da Assistência Remota.
4. Selecione **Iniciar sessão remota** para iniciar a sessão no lado do administrador.
5. Escolha baixar o formato binário do TeamViewer (Windows) e selecione **Executar**.<br/>
    **Observação** Você pode ignorar qualquer página do navegador da Web aberta no site do TeamViewer.

6. Confirme a solicitação do aplicativo TeamViewer para fazer alterações no dispositivo (somente Windows).
7. O aplicativo TeamViewer é iniciado e inclui o código de sessão para autenticar a conexão com o dispositivo remoto.

**Parte 2: No dispositivo que está sendo direcionado para uma sessão remota**

1. Implante o portal da empresa do Intune.
2. Procure um sinalizador de notificação: "O seu administrador de TI está solicitando o controle deste dispositivo para uma sessão de assistência remota" e selecione a notificação.
3. Escolha baixar o aplicativo TeamViewer ou confirme o download do aplicativo TeamViewer na App Store e selecione **Executar**.
    **Observação** Você pode ignorar qualquer página do navegador da Web aberta no site do TeamViewer.

4. Confirme a solicitação do aplicativo TeamViewer para fazer alterações no dispositivo (somente Windows).
5. O aplicativo TeamViewer é iniciado e inclui o código de sessão para autenticar a conexão com o dispositivo remoto.
6. Um pop-up pergunta se você deseja permitir que a sessão comece.

**Observação** Os códigos de sessão gerados pelo serviço TeamViewer são apenas uso único. Se você perder a conexão, você deve:

1. Fechar a instância do aplicativo TeamViewer no dispositivo remoto e na estação de trabalho do administrador.
2. Fechar o portal da empresa no dispositivo remoto.
3. Iniciar uma nova "Nova sessão de Aassistência remota" do portal de administrador.
4. Abra novamente o portal da empresa no dispositivo remoto para receber a nova notificação.
5. Baixe e abra o aplicativo TeamViewer no dispositivo remoto e na estação de trabalho de administração, como antes.