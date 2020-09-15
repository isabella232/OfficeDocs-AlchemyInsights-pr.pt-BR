---
title: Migração do Proteção de Informações do Azure para rotular MIP/Unificado no Centro de Conformidade
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674314"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migração do Proteção de Informações do Azure para rotular MIP/Unificado no Centro de Conformidade

Para migrar de etiquetas do AIP para Rotulação Unificada no entro de Segurança e Conformidade, faça o seguinte:

**Ativar a proteção do portal do Azure**

1. Se você ainda não tiver feito isso, abra uma nova janela do navegador e [entre no portal do Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Navegue até a lâmina **Proteção de Informações do Azure**. Por exemplo, no menu Hub, clique em **Todos os serviços** e comece a digitar **Informações** na Caixa de filtro. Selecione **Proteção de Informações do Azure**. Se você ainda não tiver acessado a lâmina Proteção de Informações do Azure antes, confira [etapas adicionais](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) para adicionar essa lâmina ao Portal. Para abrir a lâmina Proteção de Informações do Azure, você deve ter um [plano Premium de Proteção de Informações do Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ou um plano do Office 365 que inclui o Gerenciamento de Direitos. Se você tem uma dessas assinaturas, mas vê uma mensagem informando que não foi possível encontrar uma assinatura válida, [contate o Suporte da Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ou usar seus canais de suporte padrão.

2. Localize as opções de menu **Gerenciar** e selecione **Ativação da proteção**. Clique em **Ativar**e, em seguida, confirme a ação. Quando a ativação estiver concluída, a barra de informações exibirá **Ativação concluída com sucesso**.

**Migrar os rótulos de Proteção de Informações do Azure para o Centro de Conformidade e Segurança do Office 365**

1. Verifique se você está conectado como um usuário com permissão de Administrador Global.

2. Navegue até a lâmina **Proteção de Informações do Azure**.

3. Na opção de menu **Gerenciar**, selecione **Rotulagem Unificada**.

4. Na lâmina **Proteção de Informações do Azure - Rotulação Unificada**, clique em **Ativar** e siga as instruções online.

**Observação**: Verifique se você tem as permissões apropriadas antes de ativar a Migração do Centro de Conformidade e Segurança. Confira estes artigos para obter mais informações:

1. [Você precisa ser um administrador global do para configurar a Proteção de Informações do Azure, ou posso delegar para outros administradores?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Informações importantes sobre funções administrativas depois da migração para o Centro de Conformidade e Segurança.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Para obter mais informações sobre o AIP para rotular a migração unificada para o Centro de Conformidade e Segurança, confira [Migrar rótulos](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
