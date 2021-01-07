---
title: Proteção de dataprotection-BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768805"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitando a criptografia BitLocker com o Intune

 A política do Intune Endpoint Protection pode ser usada para definir as configurações de criptografia do BitLocker para dispositivos Windows. Para obter mais informações, consulte [configurações do Windows 10 (e posteriores) para proteger dispositivos usando o Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Você deve estar ciente de que muitos dispositivos mais recentes executando o Windows 10 dão suporte à criptografia automática do BitLocker, que é disparada sem a aplicação da política MDM. Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas. Consulte as perguntas frequentes a seguir para obter mais detalhes.
 
Para obter informações sobre a solução de problemas do BitLocker, consulte [Troubleshoot BitLocker Policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Perguntas Frequentes**

P: Quais edições do Windows dão suporte à criptografia de dispositivo usando a política do Endpoint Protection?<br>
A: as configurações na política do Intune Endpoint Protection são implementadas usando o [CSP do BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nem todas as edições ou versões do Windows dão suporte ao CSP do BitLocker. <br><br>

P: como o BitLocker pode ser habilitado nos dispositivos sem exigir interação do usuário final?<br>
A: desde que os pré-requisitos necessários sejam atendidos, é possível habilitar a "criptografia silenciosa" do BitLocker por meio do Intune. Consulte os detalhes dos requisitos do dispositivo e as configurações de política de exemplo para habilitar a criptografia silenciosa no seguinte documento: [habilitar a criptografia BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)de forma silenciosa. <br><br>

P: se um dispositivo já estiver criptografado com o BitLocker usando as configurações padrão do sistema operacional para o método de criptografia e o nível de codificação (XTS-AES-128), a aplicação de uma política com configurações diferentes disparará novamente a criptografia da unidade com as novas configurações?<br>
R: Não. Para aplicar as novas configurações de codificação, a unidade deve primeiro ser descriptografada.<br><br>
**Observação:** Para os dispositivos que estão sendo registrados com o AutoPilot, a criptografia automática que ocorre durante o OOBE não é disparada até que a política do Intune seja avaliada, o que permite que as configurações baseadas em políticas sejam usadas no lugar dos padrões do sistema operacional.
 
P: se um dispositivo for criptografado como resultado do aplicativo da política do Intune, ele será descriptografado quando essa política for removida?<br>
A: a remoção da política relacionada à criptografia não resulta na descriptografia das unidades que foram configuradas.
 
P: por que a política de conformidade do Intune mostra que meu dispositivo não tem o BitLocker habilitado, embora seja?<br>
A: a configuração "BitLocker Enabled" na política de conformidade do Intune utiliza o cliente do atestado de integridade do dispositivo Windows (DHA). Este cliente só mede o estado do dispositivo no momento da inicialização. Portanto, se um dispositivo não tiver sido reiniciado desde que a criptografia BitLocker foi concluída, o serviço de cliente DHA não relatará o BitLocker como ativo.
 
 