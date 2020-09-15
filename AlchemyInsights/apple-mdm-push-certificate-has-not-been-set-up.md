---
title: Certificado de Push MDM da Apple não foi configurado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716845"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="18812-102">Certificado de Push MDM da Apple não foi configurado</span><span class="sxs-lookup"><span data-stu-id="18812-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="18812-103">Um Certificado de Push MDM da Apple (também conhecido como um certificado de Serviço de Notificação por Push da Apple (APNS)) não foi configurado para sua assinatura.</span><span class="sxs-lookup"><span data-stu-id="18812-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="18812-104">Sem um Certificado de Push MDM da Apple configurado, você está impossibilitado de inscrever e gerenciar dispositivos com Sistemas Operacionais iOS e Mac.</span><span class="sxs-lookup"><span data-stu-id="18812-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="18812-105">Depois de adicionar o certificado ao Intune, os usuários podem instalar o aplicativo Portal da Empresa para registrar seus dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="18812-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="18812-106">Selecione **"Concordo."**</span><span class="sxs-lookup"><span data-stu-id="18812-106">Select **"I agree."**</span></span> <span data-ttu-id="18812-107">para dar permissão à Microsoft para enviar dados para a Apple.</span><span class="sxs-lookup"><span data-stu-id="18812-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="18812-108">Selecione **Baixar seu CSR** a solicitação de assinatura de certificado do Intune necessária para criar um certificado de Push MDM da Apple.</span><span class="sxs-lookup"><span data-stu-id="18812-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="18812-109">O arquivo é usado para solicitar um certificado de relação de confiança do Portal de Certificados Push da Apple.</span><span class="sxs-lookup"><span data-stu-id="18812-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="18812-110">Selecione **Criar seu Certificado Push MDM** para ir ao Portal de Certificados Push da Apple.</span><span class="sxs-lookup"><span data-stu-id="18812-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="18812-111">Entre com sua identidade empresarial da Apple e, em seguida, selecione **Criar um Certificado**.</span><span class="sxs-lookup"><span data-stu-id="18812-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="18812-112">Selecione **Escolher Arquivo**, navegue até o arquivo de solicitação de assinatura de certificado e, em seguida, escolha **Carregar**.</span><span class="sxs-lookup"><span data-stu-id="18812-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="18812-113">Na página de Confirmação, escolha **Baixar** para baixar o arquivo de certificado (.pem), e salvar o arquivo localmente.</span><span class="sxs-lookup"><span data-stu-id="18812-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="18812-114">**Observação**: O certificado está associado à Identidade da Apple usada para criá-lo.</span><span class="sxs-lookup"><span data-stu-id="18812-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="18812-115">Como prática recomendada, use uma identidade empresarial da Apple para tarefas de gerenciamento, e certifique-se que a caixa de correio está monitorada por mais de uma pessoa ou por meio de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="18812-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="18812-116">Nunca use uma identidade pessoal da Apple.</span><span class="sxs-lookup"><span data-stu-id="18812-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="18812-117">Use a mesma identidade da Apple para renovar o Certificado Push da Apple a cada 12 meses.</span><span class="sxs-lookup"><span data-stu-id="18812-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="18812-118">Insira a identidade da Apple usada para criar seu Certificado Push MDM da Apple.</span><span class="sxs-lookup"><span data-stu-id="18812-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="18812-119">Guarde essa identidade como um lembrete para quando precisar renovar o certificado.</span><span class="sxs-lookup"><span data-stu-id="18812-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="18812-120">Vá para o arquivo do certificado (.pem), escolha **Abrir** e, em seguida, escolha **Carregar**.</span><span class="sxs-lookup"><span data-stu-id="18812-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="18812-121">Com o certificado push, o Intune pode registrar e gerenciar dispositivos da Apple.</span><span class="sxs-lookup"><span data-stu-id="18812-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>