---
title: Termos ausentes do SharePoint Online Term Store
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106395"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitando a criptografia bitlocker com o Intune

A Política de Endpoint Protection do Intune pode ser usada para configurar configurações de criptografia do Boitlocker para dispositivos Windows conforme descrito em : configurações do Windows10 (e posterior) para proteger dispositivos usando o Intune

Você deve estar ciente de que muitos dispositivos mais novos que executam Windows 10 suportam criptografia automática de bitlocker que é disparada sem o aplicativo de política MDM. Isso pode afetar a aplicação da política se as configurações não padrão estão configuradas. Consulte Perguntas frequentes para obter mais detalhes.


Perguntas frequentes: Quais edições de Windows suportam a criptografia de dispositivo usando a política Endpoint Protection de segurança?
R: As configurações no Intune Endpoint Protection Política são implementadas usando o CSP do Bitlocker.  Nem todas as edições nem as builds de Windows suportam o CSP do Bitlocker. Neste momento, Windows edições: Enterprise; Education, Mobile, Mobile Enterprise e Professional (a partir da com build 1809 em diante) são suportados.




P: Se um dispositivo já estiver criptografado com o Bitlocker usando as configurações padrão do sistema operacional para o método de criptografia e a força da codificação (XTS-AES-128) aplicará uma política com configurações diferentes disparará automaticamente a nova criptografia da unidade com as novas configurações?

R: Não. Para aplicar as novas configurações de codificação, a unidade deve primeiro ser descriptografada.

Observação Para dispositivos que estão sendo inscritos no Autopilot, a criptografia automática que ocorreria durante o OOBE não é disparada até que a política do Intune seja avaliada, o que permite que as configurações baseadas em política sejam usadas no lugar dos padrões do sistema operacional




P Se um dispositivo for criptografado como resultado do aplicativo da política do Intune, ele será descriptografado quando essa política for removida?

R: A remoção da política relacionada à criptografia NÃO resulta na descriptografia das unidades que foram configuradas.




P: Por que a política de Conformidade do intune mostra que meu dispositivo não tem "Bitlocker Habilitado", mas está?

R: A configuração "Bitlocker habilitado" na política de conformidade do intune utiliza o cliente Windows DHA (Device Health Attestation). Esse cliente mede apenas o estado do dispositivo no momento da inicialização. Portanto, se um dispositivo não tiver sido reiniciado desde que a criptografia do bitlocker foi concluída, o serviço cliente DHA não informará que o bitlocker está ativo.