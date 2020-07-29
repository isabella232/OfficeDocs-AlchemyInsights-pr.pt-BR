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
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="db249-102">Usar o TeamViewer para administrar remotamente dispositivos do Intune</span><span class="sxs-lookup"><span data-stu-id="db249-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="db249-103">Os dispositivos gerenciados pelo Intune podem ser administrados remotamente usando [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="db249-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="db249-104">Para administrar o Intune usando o TeamViewer, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="db249-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="db249-105">Comece obtendo as credenciais do TeamViewer para configurar o conector do TeamViewer no Intune.</span><span class="sxs-lookup"><span data-stu-id="db249-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="db249-106">Isso permite que o administrador insira as credenciais na interface do usuário do conector do TeamViewer em dispositivos, uma operação única para estabelecer o vínculo entre o Intune e o serviço do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="db249-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="db249-107">**Parte 1: Iniciar uma sessão com um dispositivo remoto**</span><span class="sxs-lookup"><span data-stu-id="db249-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="db249-108">Em **Todos os dispositivos**, selecione o dispositivo com o qual você deseja iniciar uma sessão remota.</span><span class="sxs-lookup"><span data-stu-id="db249-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="db249-109">De **... Mais**, selecione **Nova sessão de assistência remota**.</span><span class="sxs-lookup"><span data-stu-id="db249-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="db249-110">Selecione **Sim** para confirmar que você deseja estabelecer uma sessão remota.</span><span class="sxs-lookup"><span data-stu-id="db249-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="db249-111">Após a solicitação "Iniciando uma nova sessão remota" ser reconhecida pelo serviço TeamViewer, você verá uma opção para **Iniciar a assistência remota** em detalhes do painel Visão geral (ou, Essenciais) para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db249-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="db249-112">Selecione **Ver mais** para expandir o painel e mostrar o status da Assistência Remota.</span><span class="sxs-lookup"><span data-stu-id="db249-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="db249-113">Selecione **Iniciar sessão remota** para iniciar a sessão no lado do administrador.</span><span class="sxs-lookup"><span data-stu-id="db249-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="db249-114">Escolha baixar o formato binário do TeamViewer (Windows) e selecione **Executar**.</span><span class="sxs-lookup"><span data-stu-id="db249-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="db249-115">**Observação** Você pode ignorar qualquer página do navegador da Web aberta no site do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="db249-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="db249-116">Confirme a solicitação do aplicativo TeamViewer para fazer alterações no dispositivo (somente Windows).</span><span class="sxs-lookup"><span data-stu-id="db249-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="db249-117">O aplicativo TeamViewer é iniciado e inclui o código de sessão para autenticar a conexão com o dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="db249-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="db249-118">**Parte 2: No dispositivo que está sendo direcionado para uma sessão remota**</span><span class="sxs-lookup"><span data-stu-id="db249-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="db249-119">Implante o portal da empresa do Intune.</span><span class="sxs-lookup"><span data-stu-id="db249-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="db249-120">Procure um sinalizador de notificação: "O seu administrador de TI está solicitando o controle deste dispositivo para uma sessão de assistência remota" e selecione a notificação.</span><span class="sxs-lookup"><span data-stu-id="db249-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="db249-121">Escolha baixar o aplicativo TeamViewer ou confirme o download do aplicativo TeamViewer na App Store e selecione **Executar**.</span><span class="sxs-lookup"><span data-stu-id="db249-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="db249-122">**Observação** Você pode ignorar qualquer página do navegador da Web aberta no site do TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="db249-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="db249-123">Confirme a solicitação do aplicativo TeamViewer para fazer alterações no dispositivo (somente Windows).</span><span class="sxs-lookup"><span data-stu-id="db249-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="db249-124">O aplicativo TeamViewer é iniciado e inclui o código de sessão para autenticar a conexão com o dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="db249-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="db249-125">Um pop-up pergunta se você deseja permitir que a sessão comece.</span><span class="sxs-lookup"><span data-stu-id="db249-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="db249-126">**Observação** Os códigos de sessão gerados pelo serviço TeamViewer são apenas uso único.</span><span class="sxs-lookup"><span data-stu-id="db249-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="db249-127">Se você perder a conexão, você deve:</span><span class="sxs-lookup"><span data-stu-id="db249-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="db249-128">Fechar a instância do aplicativo TeamViewer no dispositivo remoto e na estação de trabalho do administrador.</span><span class="sxs-lookup"><span data-stu-id="db249-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="db249-129">Fechar o portal da empresa no dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="db249-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="db249-130">Iniciar uma nova "Nova sessão de Aassistência remota" do portal de administrador.</span><span class="sxs-lookup"><span data-stu-id="db249-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="db249-131">Abra novamente o portal da empresa no dispositivo remoto para receber a nova notificação.</span><span class="sxs-lookup"><span data-stu-id="db249-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="db249-132">Baixe e abra o aplicativo TeamViewer no dispositivo remoto e na estação de trabalho de administração, como antes.</span><span class="sxs-lookup"><span data-stu-id="db249-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>