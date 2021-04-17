---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815603"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitando a criptografia Bitlocker com o Intune

A Política de Proteção de Ponto de Extremidade do Intune pode ser usada para configurar as configurações de criptografia do Bitlocker para dispositivos Windows. Para obter mais informações, consulte Configurações do [Windows 10 (e posteriores) para proteger dispositivos usando o Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Além da Política de Proteção de Ponto de Extremidade, há também um Relatório de Criptografia que fornece uma exibição mais detalhada do status de criptografia para dispositivos. Este relatório pode ser acessado no portal MEM em **Dispositivos > Monitor** e, em **Configuração,** selecione Relatório [de criptografia.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Se você descobrir que o Bitlocker não está habilitado conforme o esperado ou se o perfil que está sendo usado para habilitar o Bitlocker está em um estado de erro, revise o relatório de criptografia para obter uma melhor compreensão do motivo pelo qual o comportamento está ocorrendo.

Para encontrar detalhes sobre como interpretar o relatório, incluindo os vários valores de status de criptografia, consulte [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Você deve estar ciente de que muitos dispositivos mais novos que executam o Windows 10 suportam criptografia de Bitlocker automática, que é disparada sem o aplicativo de política MDM. Isso pode afetar o aplicativo de política se as configurações não padrão estão configuradas. Confira as perguntas frequentes a seguir para obter mais detalhes.

Para obter informações sobre como solucionar problemas de bitlocker, consulte [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Perguntas frequentes**

P: Quais edições do Windows suportam criptografia de dispositivo usando a Política de Proteção de Ponto de Extremidade?<br>
R: As configurações na Política de Proteção de Ponto de Extremidade do Intune são implementadas usando o [CSP bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nem todas as edições ou builds do Windows suportam o CSP do Bitlocker. <br><br>

P: Como o Bitlocker pode ser habilitado em dispositivos sem exigir a interação do usuário final?<br>
R: Desde que os pré-requisitos necessários sejam atendidos, é possível habilitar o Bitlocker "Criptografia Silenciosa" por meio do Intune. Consulte os detalhes dos requisitos de dispositivo e das configurações de política de exemplo para habilitar a criptografia silenciosa no seguinte documento: Habilitar silenciosamente a [Criptografia do Bitlocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

P: Se um dispositivo já estiver criptografado com o Bitlocker usando as configurações padrão do sistema operacional para o método de criptografia e a força da codificação (XTS-AES-128), aplicará uma política com configurações diferentes automaticamente disparará a nova criptografia da unidade com as novas configurações?<br>
R: Não. Para aplicar as novas configurações de codificação, a unidade deve primeiro ser descriptografada.<br><br>
**Observação:** Para dispositivos que estão sendo inscritos no Autopilot, a criptografia automática que ocorreria durante o OOBE não é disparada até que a política do Intune seja avaliada, o que permite que as configurações baseadas em política sejam usadas no lugar dos padrões do sistema operacional.
 
P: Se um dispositivo for criptografado como resultado do aplicativo da política do Intune, ele será descriptografado quando essa política for removida?<br>
R: A remoção da política relacionada à criptografia NÃO resulta na descriptografia das unidades que foram configuradas.
 
P: Por que a Política de Conformidade do Intune mostra que meu dispositivo não tem o Bitlocker habilitado, mesmo que seja?<br>
R: A configuração "Bitlocker habilitado" na Política de Conformidade do Intune utiliza o cliente DHA (Atestado de Saúde do Dispositivo Windows). Esse cliente mede apenas o estado do dispositivo no momento da inicialização. Portanto, se um dispositivo não tiver sido reiniciado desde que a criptografia do Bitlocker foi concluída, o serviço cliente DHA não relatará o Bitlocker como ativo.
 
 