---
title: Resolvendo erros de produtos não licenciados
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737941"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Sugestões para a solução de erros de "produto não licenciado"

Para resolver erros sobre um produto não licenciado, tente o seguinte:

- Verifique se o status da sua assinatura expirou.
- Certifique-se de que você tem uma assinatura que permite licenças de cliente, como o Microsoft 365 Apps for Business ou Business Premium, e [certifique-se de que o usuário tem uma licença atribuída](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Verifique se o usuário está entrando no Office com a mesma conta que tem a licença atribuída.
- Verifique a [página integridade do serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para ver se há algum problema conhecido com o serviço.
- Verifique o firewall, o software antivírus e as configurações de proxy para confirmar que eles não estão bloqueando o acesso aos aplicativos da Microsoft 365 para a Internet. Confira [URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Você também pode tentar as seguintes ações de solução de problemas: 

- Abra um aplicativo do Office e [saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de qualquer conta de usuário existente. [Remova](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [atribua novamente](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a licença do Office e entre no [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.
- Execute a [solução de problemas de ativação](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Reinicie o estado de ativação do Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Executar um reparo online do Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Para mais opções de solução de problemas, confira: 

- [Erros de ativação e de Produto Não Licenciado no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Erro "Não foi possível conectar-se à sua conta. Tente novamente mais tarde" ao ativar o Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)