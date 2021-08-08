---
title: 'AIP: políticas que não se comportam como esperado'
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
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934281"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: políticas que não se comportam como esperado

Proteção de Informações do Azure: para políticas que não se comportam como esperado, confira a seguir como obter diretrizes recomendadas para vários problemas de política:

1. Se você estiver tendo problemas com as marcações visuais, consulte [Quando as marcações visuais forem aplicadas](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Se você estiver tendo problemas com a rotulagem automática, consulte [Como configurar condições para a classificação automática e recomendada da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [O que os tipos de informações confidenciais procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Se você estiver tendo problemas com a proteção Nativo/Pfile, consulte [Configuração da API de arquivo](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Verifique se você está usando políticas de escopo não configuradas corretamente: [Como configurar a política de Proteção de Informações do Azure para usuários específicos usando políticas de escopo](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Se a rotulagem automática não estiver funcionando no Outlook ao anexar um documento rotulado, verifique se DRMEncryptProperty não está definido como descrito aqui: [Configurações de registro do IRM para segurança](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Se você ainda estiver enfrentando problemas, colete os logs do cliente de Proteção de Informações do Azure e anexe os logs exportados a esse tíquete.

1. Abra um documento do Office ou crie um novo email no Outlook.
2. Clique em **Proteção/Confidencialidade** > **Ajuda e comentários**.
3. Clique em **Exportar Logs**.
4. Salve os logs no local desejado e anexe-os à esta solicitação de serviço.

Recursos adicionais:

- [Como configurar um rótulo para marcações visuais da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Analisar a documentação da Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Usar rótulos de confidencialidade em aplicativos do Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

