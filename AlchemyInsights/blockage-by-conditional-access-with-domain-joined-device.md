---
title: Estou sendo bloqueado por Acesso Condicional com dispositivo associado ao domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: d71bb376615191f507d39b99d9e51ca77d929b90
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323426"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Estou sendo bloqueado por Acesso Condicional com dispositivo associado ao domínio

**Ferramentas altamente recomendadas**

[Ferramenta de Solução de Problemas de Registro de Dispositivos](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A ferramenta que ajuda a solucionar os problemas mais comuns de registro de dispositivos.

[Script de teste de conectividade de registro de dispositivo ](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - O script que ajuda a garantir que um Dispositivo possa acessar pontos de extremidade de Registro de dispositivo na conta do sistema.

[Script de limpeza de dispositivo do Azure Active Directory](https://github.com/mzmaili/AzureADDeviceCleanup) - O script que permite que você busque e gerencie dispositivos obsoletos em seu ambiente.

Aqui estão alguns motivos comuns pelos quais o acesso condicional pode falhar em um dispositivo que ingressou em um domínio (Azure Active Directory Híbrido).

1. **Não há Azure Active Directory PRT no dispositivo** - Você precisa garantir que o dispositivo tenha o Token de Atualização Primária do Azure Active Directory (PRT). Para mais informações sobre PRT, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Para verificar se você tem Azure Active Directory PRT, você pode executar o comando `dsregcmd/status` no dispositivo e verificar se “AzureAdPrt” é igual a “YES”.

Se "AzureAdPrt" for "NÃO", verifique o seguinte:

- **Se você tem um ambiente federado com AD FS e ele está inacessível nas redes domésticas de seus usuários**: neste caso, certifique-se de que seus pontos de extremidade "mesclados de usuário" estejam acessíveis a partir da extranet. Se o seu AD FS estiver atrás de uma VPN, certifique-se de que os usuários se conectem à VPN e façam login novamente no dispositivo. Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Se o TPM do dispositivo está com defeito e, portanto, não pode autenticar o dispositivo**: Verifique "tpm.msc" para ver se o estado do TPM é "Pronto". Caso contrário, execute `dsregcmd/leave` e deixe o dispositivo se reintegrar ao Azure Active Directory. Em seguida, tente novamente. Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Você está usando um provedor de identidade de terceiros, que não oferece suporte ao protocolo WS-Trust**. Conforme descrito em nossos documentos, os dispositivos híbridos associados ao Azure Active Directory não podem funcionar neste caso. Trabalhe com seu provedor de identidade para obter suporte.

2. **Os usuários estão usando o navegador Chrome sem as contas do Windows 10** ou **extensão do Office O Chrome não usa automaticamente o PRT em dispositivos AAD ou híbridos AAD**: Isso leva à falha de qualquer políticas de Acesso Condicional baseadas no dispositivo, com a mensagem de erro “Dispositivo não registrado” exibida. Para usar o navegador Chrome corretamente, você deve instalar as “Contas do Windows 10” ou "extensão do Office para o navegador Chrome dos usuários" via SCCM ou Intune. Para obter mais informações, confira este [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Se não for possível enviar a extensão remotamente, notifique os usuários para instalar manualmente uma das extensões acima para acessar aplicativos por meio de Acesso Condicional baseado no dispositivo. Para mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **O dispositivo foi corretamente ingressado no Azure AD híbrido, mas foi inadvertidamente excluído ou desabilitado, devido a alterações de sincronização no Azure AD Connect ou no portal do Azure**: Se isso acontecer, o objeto de dispositivo não será mais reconhecido como um dispositivo totalmente unido, embora os status "AzureAdJoined" e "PRT" apareçam como válidos no dispositivo.

Para corrigir esse problema, execute `dsregcmd/leave` nos dispositivos afetados e deixe-os reingressar no Azure Active Directory. Para mais informações, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

**Observação**: se seus dispositivos estiverem no Windows 10, atualização 1809, com VPN/Cloud Proxy e virem problemas com o estado "AzureAdPrt" ou qualquer aplicativo com problema de SSO (perspectiva de não conectar à caixa de correio mesmo que você tenha PRT), certifique-se de ter este patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ou atualização cumulativa de abril [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) para evitar falhas de PRT nessas máquinas.

















