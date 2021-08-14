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
ms.openlocfilehash: 4f8e3502a7be35b5579ec1436852fe2bff9b1316891c7a9020f6f5f4767b3d88
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931510"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Certificado de Push MDM da Apple não foi configurado

Um Certificado de Push MDM da Apple (também conhecido como um certificado de Serviço de Notificação por Push da Apple (APNS)) não foi configurado para sua assinatura. Sem um Certificado de Push MDM da Apple configurado, você está impossibilitado de inscrever e gerenciar dispositivos com Sistemas Operacionais iOS e Mac. Depois de adicionar o certificado ao Intune, os usuários podem instalar o aplicativo Portal da Empresa para registrar seus dispositivos iOS.

1. Selecione **"Concordo."** para dar permissão à Microsoft para enviar dados para a Apple.

2. Selecione **Baixar seu CSR** a solicitação de assinatura de certificado do Intune necessária para criar um certificado de Push MDM da Apple. O arquivo é usado para solicitar um certificado de relação de confiança do Portal de Certificados Push da Apple.

3. Selecione **Criar seu Certificado Push MDM** para ir ao Portal de Certificados Push da Apple. Entre com sua identidade empresarial da Apple e, em seguida, selecione **Criar um Certificado**. Selecione **Escolher Arquivo**, navegue até o arquivo de solicitação de assinatura de certificado e, em seguida, escolha **Carregar**. Na página de Confirmação, escolha **Baixar** para baixar o arquivo de certificado (.pem), e salvar o arquivo localmente.
 
**Observação**: O certificado está associado à Identidade da Apple usada para criá-lo. Como prática recomendada, use uma identidade empresarial da Apple para tarefas de gerenciamento, e certifique-se que a caixa de correio está monitorada por mais de uma pessoa ou por meio de uma lista de distribuição. Nunca use uma identidade pessoal da Apple. Use a mesma identidade da Apple para renovar o Certificado Push da Apple a cada 12 meses.
 
4. Insira a identidade da Apple usada para criar seu Certificado Push MDM da Apple. Guarde essa identidade como um lembrete para quando precisar renovar o certificado.

5. Vá para o arquivo do certificado (.pem), escolha **Abrir** e, em seguida, escolha **Carregar**. Com o certificado push, o Intune pode registrar e gerenciar dispositivos da Apple.