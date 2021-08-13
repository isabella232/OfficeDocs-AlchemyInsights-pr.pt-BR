---
title: Não é possível ativar o Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928357"
---
# <a name="unable-to-activate-office"></a>Não é possível ativar o Office

**Observação**: se você estiver usando uma versão mais antiga do Windows (Por exemplo, Windows 7), certifique-se de que o TLS 1.2 está habilitado como padrão. Para obter mais informações, confira [Atualizar para habilitar o TLS 1.1 e o TLS 1.2 como protocolos seguros padrão em WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

- Verifique se o status da sua assinatura expirou.
- Certifique-se de ter uma assinatura que permita licenças de cliente, como o Office 365 Business ou Business Premium, e [garanta que o usuário tenha uma licença atribuída](/microsoft-365/admin/manage/assign-licenses-to-users).
- Certifique-se de que o usuário esteja entrando no Office com a mesma conta para a qual a assinatura foi atribuída.
- Verifique a [página de integridade do serviço do Office 365](/office365/enterprise/view-service-health) para ver se há algum problema conhecido com o serviço.
- Verifique o firewall, software antivírus e as configurações do proxy para confirmar se eles não estão bloqueando o acesso dos aplicativos Microsoft 365 à Internet. Confira os [URLs do Office 365 e os intervalos de endereços IP](/office365/enterprise/urls-and-ip-address-ranges "Intervalos de endereços IP e URLs do Office 365").

**Dica** em computadores com Windows, podemos diagnosticar e corrigir automaticamente vários problemas de entrada comuns do Office para você. Baixe e execute o  **[Assistente de Suporte e Recuperação da Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para usar nossa ferramenta automatizada.

Siga estas instruções para solucionar o problema:

- Abra um aplicativo do Office e [saia](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) das contas de usuários existentes. [Remova](/microsoft-365/admin/manage/remove-licenses-from-users) e [reatribua](/microsoft-365/admin/manage/assign-licenses-to-users) a licença do Office e, em seguida, [entre no Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) usando a conta de usuário afetada.
- Execute a [Solução de Problemas de Ativação](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Reinicie o estado de ativação do Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reiniciar o estado de ativação do Office")
- [Execute um Reparo Online do Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Para mais opções de solução de problemas, confira:  

- [Erros de ativação e de Produto Não Licenciado no Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Erro "Não foi possível conectar-se à sua conta. Tente novamente mais tarde" ao ativar o Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)