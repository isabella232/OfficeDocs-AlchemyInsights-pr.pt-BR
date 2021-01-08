---
title: DataProtection - Bitlocker
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
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778181"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitando a criptografia Bitlocker com o Intune

A Política de Proteção de Ponto de Extremidade do Intune pode ser usada para definir as configurações de criptografia do Bitlocker para dispositivos Windows. Para obter mais informações, consulte [as configurações do Windows 10 (e posteriores) para proteger dispositivos usando o Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Além da Política de Proteção de Ponto de Extremidade, há também um Relatório de Criptografia que fornece uma exibição mais detalhada do status de criptografia para dispositivos. Esse relatório pode ser acessado no portal do MEM em **Dispositivos > Monitor** e, em Configuração, **selecione** Relatório [de criptografia.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Se você achar que o Bitlocker não está habilitado conforme o esperado ou se o perfil que está sendo usado para habilitar o Bitlocker está em um estado de erro, revise o relatório de criptografia para entender melhor por que o comportamento está ocorrendo.

Para encontrar detalhes sobre como interpretar o relatório, incluindo os vários valores de status de criptografia, consulte Monitorar a criptografia de dispositivo [com o Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Você deve estar ciente de que muitos dispositivos mais novos que executam o Windows 10 suportam a criptografia automática do Bitlocker, que é disparada sem o aplicativo da política MDM. Isso poderá afetar a aplicação da política se as configurações não padrão são configuradas. Consulte as perguntas frequentes a seguir para obter mais detalhes.

Para obter informações sobre como solucionar problemas do bitlocker, consulte Solucionar problemas de políticas [do BitLocker no Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Perguntas Frequentes**

P: Quais edições do Windows suportam criptografia de dispositivo usando a Política de Proteção de Ponto de Extremidade?<br>
R: As configurações na Política de Proteção de Ponto de Extremidade do Intune são implementadas usando o [CSP do Bitlocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nem todas as edições ou builds do Windows são suportadas pelo CSP do Bitlocker. <br><br>

P: Como o Bitlocker pode ser habilitado em dispositivos sem a necessidade de interação do usuário final?<br>
R: Desde que os pré-requisitos necessários sejam atendidos, é possível habilitar a "Criptografia Silenciosa" do Bitlocker por meio do Intune. Consulte os detalhes dos requisitos de dispositivo e das configurações de política de exemplo para habilitar a criptografia silenciosa no seguinte documento: Habilitar silenciosamente [a Criptografia do Bitlocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

P: Se um dispositivo já estiver criptografado com o Bitlocker usando as configurações padrão do sistema operacional para o método de criptografia e o nível de codificação (XTS-AES-128), a aplicação de uma política com configurações diferentes disparará automaticamente a nova criptografia da unidade com as novas configurações?<br>
R: Não. Para aplicar as novas configurações de codificação, a unidade deve ser descriptografada primeiro.<br><br>
**Observação:** Para dispositivos que estão sendo inscritos no Autopilot, a criptografia automática que ocorreria durante o OOBE não é disparada até que a política do Intune seja avaliada, o que permite que as configurações baseadas em política sejam usadas no lugar dos padrões do sistema operacional.
 
P: Se um dispositivo for criptografado como resultado do aplicativo da política do Intune, ele será descriptografado quando essa política for removida?<br>
R: A remoção da política relacionada à criptografia NÃO resulta na descriptografia das unidades que foram configuradas.
 
P: Por que a Política de Conformidade do Intune mostra que meu dispositivo não tem o Bitlocker habilitado, mesmo que ele seja?<br>
R: A configuração "Bitlocker habilitado" na Política de Conformidade do Intune utiliza o cliente do Atestado de Saúde do Dispositivo Windows (DHA). Esse cliente mede apenas o estado do dispositivo no momento da inicialização. Portanto, se um dispositivo não tiver sido reiniciado desde que a criptografia Bitlocker foi concluída, o serviço cliente do DHA não relatará o Bitlocker como ativo.
 
 