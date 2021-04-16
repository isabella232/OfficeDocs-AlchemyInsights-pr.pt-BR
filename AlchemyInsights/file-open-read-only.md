---
title: Somente leitura de arquivo aberto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813172"
---
# <a name="file-open-read-only"></a><span data-ttu-id="42bd4-102">Somente leitura de arquivo aberto</span><span class="sxs-lookup"><span data-stu-id="42bd4-102">File open read-only</span></span>

<span data-ttu-id="42bd4-103">Você pode descobrir que, ao abrir arquivos, eles são abertos como somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42bd4-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="42bd4-104">Em alguns casos, isso é para maior segurança, como quando você está abrindo arquivos da Internet e outras vezes, pode ser devido a uma configuração que pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="42bd4-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="42bd4-105">Aqui estão alguns cenários em que um arquivo abre somente leitura e algumas etapas que você pode seguir para alterar isso.</span><span class="sxs-lookup"><span data-stu-id="42bd4-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="42bd4-106">**Meu antivírus está fazendo com que eles abram somente leitura**</span><span class="sxs-lookup"><span data-stu-id="42bd4-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="42bd4-107">Alguns programas antivírus podem protegê-lo contra arquivos potencialmente não seguros abrindo-os somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42bd4-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="42bd4-108">Talvez seja necessário verificar com seu provedor de antivírus para saber como ajustar essas configurações.</span><span class="sxs-lookup"><span data-stu-id="42bd4-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="42bd4-109">BitDefender, por exemplo, tem conteúdo sobre como adicionar exclusões de aplicativos aqui: Como adicionar exclusões de aplicativo ou processo no Centro de Controle [Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="42bd4-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="42bd4-110">**As propriedades do arquivo são definidas como somente leitura?**</span><span class="sxs-lookup"><span data-stu-id="42bd4-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="42bd4-111">Você pode verificar as propriedades do arquivo clicando com o botão direito do mouse no arquivo e escolhendo Propriedades.</span><span class="sxs-lookup"><span data-stu-id="42bd4-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="42bd4-112">Se o atributo Somente leitura for verificado, você poderá desmarcar e clicar em OK.</span><span class="sxs-lookup"><span data-stu-id="42bd4-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="42bd4-113">**O conteúdo está em exibição protegida**</span><span class="sxs-lookup"><span data-stu-id="42bd4-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="42bd4-114">Arquivos da Internet e de outros locais potencialmente não seguros podem conter vírus, worms ou outros tipos de malware que podem prejudicar seu computador.</span><span class="sxs-lookup"><span data-stu-id="42bd4-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="42bd4-115">Isso também acontece normalmente com anexos de email ou arquivos que você baixou.</span><span class="sxs-lookup"><span data-stu-id="42bd4-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="42bd4-116">Para ajudar a proteger seu computador, os arquivos desses locais potencialmente não seguros são abertos no Protected View.</span><span class="sxs-lookup"><span data-stu-id="42bd4-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="42bd4-117">Usando o Protected View, você pode ler um arquivo e ver seu conteúdo ao reduzir os riscos.</span><span class="sxs-lookup"><span data-stu-id="42bd4-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="42bd4-118">Para obter mais informações sobre o exibição protegido e como alterar as configurações, consulte este artigo: [O que é Exibição Protegida?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="42bd4-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="42bd4-119">**O OneDrive está completo?**</span><span class="sxs-lookup"><span data-stu-id="42bd4-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="42bd4-120">Se o arquivo for armazenado no OneDrive e seu espaço de armazenamento do OneDrive estiver cheio, você não poderá salvar o documento até que você está sob seu espaço alocado.</span><span class="sxs-lookup"><span data-stu-id="42bd4-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="42bd4-121">Você pode verificar seu espaço livre no OneDrive clicando no ícone do OneDrive no centro de notificação e escolhendo Gerenciar armazenamento, ou você pode ir para , entrar e observar a quantidade de espaço usado na parte inferior esquerda da [https://onedrive.live.com](https://onedrive.live.com) tela.</span><span class="sxs-lookup"><span data-stu-id="42bd4-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="42bd4-122">**O Office está ativado?**</span><span class="sxs-lookup"><span data-stu-id="42bd4-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="42bd4-123">Se o Office não estiver ativado ou se sua assinatura tiver expirado, você poderá estar no Modo de Funcionalidade Reduzida somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42bd4-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="42bd4-124">Para obter informações sobre como ativar o Office, consulte: Erros de ativação e produto sem licença [no Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="42bd4-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="42bd4-125">**Se todo o resto falhar...**</span><span class="sxs-lookup"><span data-stu-id="42bd4-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="42bd4-126">Tente reiniciar o computador</span><span class="sxs-lookup"><span data-stu-id="42bd4-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="42bd4-127">Instalar atualizações do Office</span><span class="sxs-lookup"><span data-stu-id="42bd4-127">Install Office updates</span></span>
    
- <span data-ttu-id="42bd4-128">Executar um reparo online do Office</span><span class="sxs-lookup"><span data-stu-id="42bd4-128">Perform an Online repair of Office</span></span>
    

