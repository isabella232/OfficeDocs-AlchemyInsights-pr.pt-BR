---
title: Solução de erros de produto não-licença
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786837"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Sugestões para resolver erros de "Produto Sem Licença"

Para resolver erros sobre um "Produto Sem Licença", tente o seguinte:

- Verifique se o status da sua assinatura expirou.
- Certifique-se de ter uma assinatura que permita licenças de cliente, como o Microsoft 365 Apps para empresas ou o Business Premium, e verifique se o usuário tem uma licença atribuída [.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Certifique-se de que o usuário está se insinuando no Office com a mesma conta que tem a licença atribuída.
- Verifique a [página de saúde do serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para ver se há algum problema conhecido com o serviço.
- Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando o acesso de aplicativos do Microsoft 365 à Internet. Consulte [URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Você também pode tentar as seguintes ações de solução de problemas: 

- Abra um aplicativo do Office [e saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de qualquer conta de usuário existente. [Remova](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [atribua a licença](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) do Office e entre no [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.
- Execute o [Solução de Problemas de Ativação](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Reinicie o estado de ativação do Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Execute um Reparo Online do Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Para mais opções de solução de problemas, confira: 

- [Erros de ativação e de Produto Não Licenciado no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Erro "Não foi possível conectar-se à sua conta. Tente novamente mais tarde" ao ativar o Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)