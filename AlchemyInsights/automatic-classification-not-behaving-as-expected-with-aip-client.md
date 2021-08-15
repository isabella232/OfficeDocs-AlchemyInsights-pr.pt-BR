---
title: Classificação automática não se comportando como esperado com o cliente AIP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979697"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Classificação automática não se comportando como esperado com o cliente AIP

Use as diretrizes a seguir, quando a classificação automática não estiver se comportando como esperado:

1. Se você estiver tendo problemas com a rotulagem automática, confira [Como configurar condições para a classificação automática e recomendada da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [O que os tipos de informações confidenciais procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Verifique se você está usando políticas de escopo não configuradas corretamente: [Como configurar a política de Proteção de Informações do Azure para usuários específicos usando políticas de escopo](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Se a rotulagem automática não estiver funcionando no Outlook ao anexar um documento rotulado, verifique se `DRMEncryptProperty` não está definido como descrito aqui: [Configurações de registro do IRM para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Se você usou os [tipos de informações internas](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) para a política de Proteção de Informações do Azure, verifique se o seu conteúdo corresponde ao formato esperado.
5. Verifique se o rótulo está configurado adequadamente como **Automático** ou **Recomendado**. (A rotulagem **automática** está disponível para todos os aplicativos do Microsoft 365, enquanto a **Recomendada** está disponível para todos os aplicativos do Microsoft 365, exceto o Outlook.)
6. Você não pode usar a classificação automática para documentos e emails que foram anteriormente rotulados manualmente ou automaticamente com uma classificação mais alta.  Para obter mais informações, confira: [Como as rótulos automáticos ou recomendados são aplicados](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Se você ainda estiver com enfrentando problemas, colete os logs do cliente de Proteção de Informações do Azure e anexe os logs exportados ao tíquete de suporte. Para exportar os logs da Proteção de Informações do Azure:
    - Abra um documento do Office ou crie um novo email no Outlook.
    - Clique em **Proteção/Confidencialidade** > **Ajuda e comentários**.
    - Clique em **Exportar Logs**.
    - Salve os logs no local desejado e anexe-os à sua solicitação de serviço.

Confira mais informações em:

- [Como configurar condições para classificação automática e recomendada para a Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Guias de instruções para cenários comuns que usam a Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Analisar a documentação da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Analisar as assinaturas e os recursos da Proteção de Informações do Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Requisitos da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements).
- [Tutorial de início rápido da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).
- [Baixar o cliente da Proteção de Informações do Azure](https://www.microsoft.com/download/details.aspx?id=53018)
