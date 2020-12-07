---
title: Habilitar o write-back de senha no Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560428"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="47cba-102">Habilitar o write-back de senha no Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="47cba-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="47cba-103">Para habilitar o write-back da redefinição de senha por autoatendimento, habilite primeiro a opção de write-back no Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="47cba-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="47cba-104">A partir do seu servidor do Azure AD Connect, realize as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="47cba-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="47cba-105">Entre no seu servidor Azure AD Connect e inicie o assistente de configuração do **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="47cba-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="47cba-106">Na página **Bem-vindo**, clique em **Configurar**.</span><span class="sxs-lookup"><span data-stu-id="47cba-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="47cba-107">Na página **Tarefas adicionais**, clique em **Personalizar as opções de sincronização** e depois em **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="47cba-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="47cba-108">Na página Conectar ao Azure AD, insira uma credencial de administrador global para o locatário do Azure e clique em Avançar.</span><span class="sxs-lookup"><span data-stu-id="47cba-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="47cba-109">Nas páginas **Conectar os diretórios** e **Filtrar domínio/UO**, clique em **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="47cba-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="47cba-110">Na página **Recursos opcionais**, selecione a caixa ao lado de **Write-back de senha** e clique em **Avançar**.</span><span class="sxs-lookup"><span data-stu-id="47cba-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="47cba-111">Na página **Pronto para configurar**, clique em **Configurar** e aguarde que o processo seja concluído.</span><span class="sxs-lookup"><span data-stu-id="47cba-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="47cba-112">Ao concluir a configuração, clique em **Sair**.</span><span class="sxs-lookup"><span data-stu-id="47cba-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="47cba-113">Com o write-back de senha habilitado no Azure AD Connect, agora poderá configurar o SSPR do Azure AD para write-back.</span><span class="sxs-lookup"><span data-stu-id="47cba-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="47cba-114">Para habilitar o writeback de senha no SSPR, conclua as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="47cba-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="47cba-115">Entre no portal do Azure usando uma conta de administrador global.</span><span class="sxs-lookup"><span data-stu-id="47cba-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="47cba-116">Pesquise e selecione o **Azure Active Directory**, clique em **Redefinição de senha** e escolha **Integração local**.</span><span class="sxs-lookup"><span data-stu-id="47cba-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="47cba-117">Definir a opção **Gravar as senhas em seu diretório local?** para **Sim**.</span><span class="sxs-lookup"><span data-stu-id="47cba-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="47cba-118">Defina a opção **Permitir que os usuários desbloqueiem contas sem redefinir a senha?** para **Sim**.</span><span class="sxs-lookup"><span data-stu-id="47cba-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="47cba-119">Quando estiver pronto, clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="47cba-119">When ready, click **Save**.</span></span>

<span data-ttu-id="47cba-120">Para saber mais, confira [Habilitar o write-back da redefinição de senha por autoatendimento do Azure Active Directory em um ambiente local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="47cba-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="47cba-121">Quando um administrador redefine a senha de um usuário no portal do Microsoft Azure, se esse usuário for federado ou hash de senha sincronizada, a senha será gravada no local.</span><span class="sxs-lookup"><span data-stu-id="47cba-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="47cba-122">Atualmente, não há suporte para esta funcionalidade no portal de Administração do Office.</span><span class="sxs-lookup"><span data-stu-id="47cba-122">This functionality is currently not supported in the Office Admin portal.</span></span>