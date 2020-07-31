---
title: Solução de problemas na implantação do certificado de autenticação do cliente
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509036"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Solução de problemas na implantação do certificado de autenticação do cliente

Os perfis Intune NDES/SCEP e PKCS/PFX de certificados de clientes são normalmente usados em conjunto com outros tipos de perfis, como Wi-Fi, VPN e e-mails, para permitir que os usuários autentiquem os recursos corporativos. Quando esses tipos de perfil estão ligados a um perfil de certificado de cliente, dependem do sucesso da implantação desse perfil.

A configuração inicial da infraestrutura e a configuração associada do perfil do Certificado do cliente normalmente exigem a solução de problemas. Para obter um guia passo a passo para a configuração bem-sucedida do conector NDES e orientações de solução de problemas para isolar problemas com a implantação de certificados, consulte: 

- [Configurar a infraestrutura para oferecer suporte ao SCEP com o Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Visão geral da solução de problemas dos perfis de certificados SCEP com o Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Usar os scripts do Powershell referenciados para ajudar a verificar sua configuração. Para obter ais informações, consulte [Scripts de verificação de conectores Intune Certificate](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Outros problemas comuns**

**Quando tento instalar o conector do certificado Intune no servidor do conector NDES, recebo a mensagem: "A senha no pedido de certificado não pode ser verificada. Ela já pode ter sido usada. Obtenha uma nova senha para enviar com esta solicitação".**  

Essa mensagem quer dizer que você precisa executar a instalação do conector do certificado como Administrador.

Em alguns ambientes, os servidores onde o Certificado Intune é executado devem usar um servidor proxy para se conectarem ao Intune e, assim, o Conector do Certificado deve usar um proxy. Em algumas circunstâncias, o Conector NDES ignora as configurações de proxy configuradas, e talvez seja necessário configurar as configurações de proxy enquanto estiver em execução no contexto de segurança do LocalSystem. 
 
A solução é executar o Internet Explorer como SISTEMA e configurar um proxy no IE. Depois de reiniciar o Serviço de Conector Intune, o Conector NDES se conecta ao Intune.

**Os dispositivos do usuário não estão mais recebendo certificados SCEP da NDES.**

É possível que o certificado de Autenticação do Cliente emitido para o servidor NDES, e especificado durante a instalação do conector NDES, tenha expirado ou esteja desaparecido. Para resolver: 
 
1. Desinstalar o conector NDES.  
2. Usar estes detalhes para solicitar uma nova autenticação de cliente ou um certificado de autenticação de servidor: 
 
    - Nome do assunto: CN=fqdn externo  
    - Nome alternativo ao assunto (ambos são necessários): DNS=fqdn externo, DNS=fqdn interno 
 
3. Reinstalar o conector NDES com o novo certificado.