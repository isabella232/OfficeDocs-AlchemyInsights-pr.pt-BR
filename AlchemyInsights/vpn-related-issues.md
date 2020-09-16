---
title: Problemas relacionados à VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726079"
---
# <a name="vpn-related-issues"></a>Problemas relacionados à VPN

A implementação bem-sucedida da conectividade VPN para clientes MDM depende de um perfil implantado que reflete corretamente os requisitos da infraestrutura VPN. Para configurar adequadamente as plataformas de cliente que está investigando, confira: 

[Configurações de dispositivo do Windows 10 e Windows Holographic para adicionar conexões de VPN usando o Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Adicionar configurações de VPN a dispositivos iOS e iPadOS no Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Configurações de dispositivo Android para configurar a VPN no Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Adicionar configurações de VPN a dispositivos macOS no Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Se seu perfil VPN usar autenticação baseada em certificado, garanta que o certificado raiz e os perfis de certificado de autenticação de cliente vinculados ao perfil VPN sejam implantados com êxito.

**Problemas Comuns**

**Implantei um perfil VPN em um dispositivo. O Intune está mostrando que foi bem-sucedido, mas o dispositivo não está se conectando à VPN.**

Um status bem-sucedido significa que o Intune implantou o perfil configurado com êxito. No entanto, essas configurações podem não corresponder aos requisitos de rede e/ou autenticação. Examine os logs no serviço de infraestrutura e de autenticação (no servidor VPN e no servidor NPS/Radius) para obter mais detalhes sobre a tentativa de conexão. Talvez você precise trabalhar com sua equipe de infraestrutura de rede ou com o fornecedor de VPN de terceiros para reunir e analisar os logs.

**Quando configuro uma VPN personalizada para iOS, o recurso VPN por aplicativo não é disponibilizado.**

A VPN por aplicativo para dispositivos iOS no Intune está disponível no momento para uma lista específica de provedores e parceiros, que também devem atender aos pré-requisitos de certificado antes de configurar uma VPN por aplicativo. Para saber mais, veja [Configurar VPN (Rede Virtual Privada) por aplicativo para dispositivos iOS/iPadOS no Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Para saber mais informações sobre todos os tipos de conexão VPN no Intune, veja [Criar perfis VPN para se conectar aos servidores VPN no Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**A VPN sob demanda do iOS não inicia quando um domínio configurado é acessado**

Para testar as configurações VPN automáticas, defina os valores a seguir:

Quero fazer o seguinte: **Avaliar todas as tentativas de conexão** 

Escolha se deseja se conectar: **Conectar, se necessário**

Quando usuários acessam esses domínios: **destino** *nome de domínio*

Se a configuração acima não tiver êxito, adicione o seguinte elemento:

Quando essa URL estiver inatingível, force a conexão com a VPN: **BADURL**