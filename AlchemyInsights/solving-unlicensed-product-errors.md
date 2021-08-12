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
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957088"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Sugestões para resolver erros de "Produto Sem Licença"

Para resolver erros sobre um "Produto Sem Licença", tente o seguinte:

- Verifique se o status da sua assinatura expirou.
- Certifique-se de ter uma assinatura que permita licenças de cliente, como Microsoft 365 Apps para Pequenos e Médios negócios ou Business Premium, e certifique-se de que o usuário tenha uma licença [atribuída](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Certifique-se de que o usuário está Office com a mesma conta atribuída.
- Verifique a [página de saúde do serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para ver se há algum problema conhecido com o serviço.
- Verifique as configurações de firewall, software antivírus e proxy para confirmar se eles não estão bloqueando Microsoft 365 acesso de aplicativos à Internet. Consulte [URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Você também pode tentar as seguintes ações de solução de problemas: 

- Abra um Aplicativo do Office [e saia de](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) qualquer conta de usuário existente. [Remova](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [atribua a Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) e, em seguida, entre no Office [usando](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) a conta de usuário afetada.
- Execute o [Solução de Problemas de Ativação](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Reinicie o estado de ativação do Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Execute um Reparo Online de Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Para mais opções de solução de problemas, confira: 

- [Erros de ativação e de Produto Não Licenciado no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Erro "Não foi possível conectar-se à sua conta. Tente novamente mais tarde" ao ativar o Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)