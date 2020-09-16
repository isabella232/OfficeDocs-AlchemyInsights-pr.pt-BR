---
title: Não é possível ativar o Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 50939456df57920994e464db20e5da54f45f197a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744614"
---
# <a name="unable-to-activate-office"></a>Não é possível ativar o Office

- Verifique se o status da sua assinatura expirou.
- Certifique-se de ter uma assinatura que permita licenças de cliente, como o Office 365 Business ou Business Premium, e [garanta que o usuário tenha uma licença atribuída](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).
- Certifique-se de que o usuário esteja entrando no Office com a mesma conta para a qual a assinatura foi atribuída.
- Verifique a [página de integridade do serviço do Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) para ver se há algum problema conhecido com o serviço.
- Verifique as configurações de firewall, software antivírus e proxy para verificar se eles estão bloqueando o acesso de aplicativos do Microsoft 365 à Internet. Confira [URLs e intervalos de endereços IP do Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Intervalos de endereços IP e URLs do Office 365").

Siga estas instruções para solucionar o problema:

- Abra um aplicativo do Office e [saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) das contas de usuários existentes. [Remova](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [reatribua](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a licença do Office e, em seguida, [entre no Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.
- Execute a [Solução de Problemas de Ativação](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Reinicie o estado de ativação do Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reiniciar o estado de ativação do Office")
- [Execute um Reparo Online do Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Para mais opções de solução de problemas, confira:  

- [Erros de ativação e de Produto Não Licenciado no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Erro "Não foi possível conectar-se à sua conta. Tente novamente mais tarde" ao ativar o Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)