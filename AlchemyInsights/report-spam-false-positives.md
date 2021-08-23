---
title: Você gostaria de relatar um falso positivo de spam para a Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396603"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Você tem mensagens legítimas marcadas como spam?

É frustrante quando um email legítimo termina na pasta Lixo Eletrônico ou em Quarentena. Considere estes motivos mais comuns para falsos positivos:

**Substituições de locatários (mais comuns)** Isso está totalmente dentro do seu controle para correção.

Enviar a mensagem no Microsoft 365 Defender para análise das políticas e regras que impactam; Os detalhes da varredura rescan estão disponíveis em minutos.
Revise ou modifique as políticas ou regras conforme aplicável. 

**Substituições do usuário final (comum)** Isso está totalmente dentro do seu controle para correção. 

Enviar a mensagem no Microsoft 365 Defender para análise das políticas e regras que impactam; Os detalhes da varredura rescan estão disponíveis em minutos. 

Se uma mensagem foi bloqueada porque foi enviada de um endereço na lista remetentes bloqueados de um usuário, os headers incluem o Veredito de Filtragem de Spam "SFV:BLK".

**Autenticação de email dos envios** Isso está parcialmente dentro do seu controle para correção.

Enviar a mensagem para analisar falhas na autenticação de email do remetente no momento da entrega; os resultados estão disponíveis em um dia. 

Se você possui a infraestrutura de envio, revise como alinhe-a com SPF, DKIM e DMARC para garantir que os sistemas de email de destino confiem em mensagens enviadas de seu domínio. Como alternativa, contate os remetentes para tratar de suas configurações DNS.

**Vereditos de filtragem da Microsoft** Isso está parcialmente dentro do seu controle para correção.

Enviar a mensagem e relatar a mensagem como segura; Os resultados da varredura rescan estão disponíveis dentro de um dia. Use a Lista de Locatários Permitir/Bloquear quando você não concordar com os vereditos de filtragem em situações específicas. No entanto, você não deve ignorar os vereditos de filtragem da Microsoft permanentemente. 

Para mais informações, confira:

- Habilita os usuários finais a enviar mensagens à Microsoft. A Microsoft usa esses envios para melhorar a eficácia das tecnologias de proteção de email, e elas aparecem em relatórios de envio para você usar como uma indicação para atualizar políticas. 

- Para assistir a um breve vídeo ao enviar mensagens para análise, consulte [Enviando mensagens para análise](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Usar o Envio do Administrador para enviar spam, phishing, URLs e arquivos à Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Gerenciar a lista de Permissões/Bloqueios do Locatário](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Cabeçalhos de mensagens anti-spam no Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Proteção contra spam de saída no EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)