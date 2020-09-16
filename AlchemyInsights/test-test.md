---
title: Termos ausentes do repositório de termos do SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750439"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitando a criptografia BitLocker com o Intune

A política do Intune Endpoint Protection pode ser usada para definir configurações de criptografia do Boitlocker para dispositivos Windows, conforme descrito em: Windows10 (e posterior) configurações para proteger dispositivos usando o Intune

Você deve estar ciente de que muitos dispositivos mais recentes que executam o Windows 10 dão suporte à criptografia automática do BitLocker, que é disparada sem a aplicação da política de MDM. Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas. Confira mais detalhes na seção perguntas frequentes.


Perguntas frequentes   p: Quais edições do Windows dão suporte à criptografia de dispositivo usando a política do Endpoint Protection?
 A: as configurações na política do Intune Endpoint Protection são implementadas usando o CSP do BitLocker.Nem todas as edições nem versões do Windows dão suporte ao CSP do BitLocker. 
      No momento, edições do Windows: Enterprise; Educação, Mobile, Mobile Enterprise e Professional (da compilação 1809 em diante) são suportados.




P: se um dispositivo já estiver criptografado com o BitLocker usando as configurações padrão do sistema operacional para o método de criptografia e o nível de codificação (XTS-AES-128), a aplicação de uma política com configurações diferentes disparará novamente a criptografia da unidade com as novas configurações?

R: Não. Para aplicar as novas configurações de codificação, a unidade deve primeiro ser descriptografada.

Observação para os dispositivos que estão sendo registrados com o AutoPilot a criptografia automática que ocorre durante o OOBE não é disparada até que a política do Intune seja avaliada, o que permite que as configurações baseadas em políticas sejam usadas no lugar dos padrões do sistema operacional




P se um dispositivo for criptografado como resultado do aplicativo da política do Intune, ele será descriptografado quando essa política for removida?

A: a remoção da política relacionada à criptografia não resulta na descriptografia das unidades que foram configuradas.




P: por que a política de conformidade do Intune mostra que meu dispositivo não tem "BitLocker habilitado", mas é?

A: a configuração "BitLocker Enabled" na política de conformidade do Intune utiliza o cliente do atestado de integridade do dispositivo Windows (DHA). Este cliente só mede o estado do dispositivo no momento da inicialização. Portanto, se um dispositivo não tiver sido reiniciado desde que a criptografia BitLocker foi concluída, o serviço de cliente DHA não relatará o BitLocker como ativo.