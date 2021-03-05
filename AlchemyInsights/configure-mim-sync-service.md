---
title: Configurar o serviço de Sincronização MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430707"
---
# <a name="configure-mim-sync-service"></a>Configurar o serviço de Sincronização MIM

O Serviço de Sincronização Microsoft Identity Manager (MIM) é um componente do MIM. É um serviço local centralizado que armazena e integra informações para organizações que possuem vários diretórios e bancos de dados locais. Você pode resolver o seu problema com a Sincronização MIM se o problema foi abordado em uma atualização recente do MIM ou se for um dos outros problemas mencionados na seção abaixo.

**Etapas recomendadas**

1. Certifique-se de estar usando uma atualização recente da Sincronização MIM e verifique as [observações de versão da Sincronizar MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) para determinar se o problema foi resolvido em uma atualização.
2. Se o problema for com o conector LDAP Genérico, SQL Genérico, Lotus Domino ou conector de Serviços Web, certifique-se de estar usando uma atualização recente dos [conectores genéricos](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Se a execução de uma Sincronização MIM parar com um erro, consulte a tabela de [códigos de erro de execução](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) para determinar as causas potenciais.
4. Se a execução for interrompida com a **exceção de extensão dll**, clique nessas palavras para abrir a janela **Propriedades do Objeto do Espaço Conector** e clique em **Rastreamento de Pilha...** para consultar mais informações sobre a causa subjacente, conforme descrito na [Exceção de Extensão DLL](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Se o componente Serviço de Notificação de alteração de Senha (PCNS) relatar o **erro 6025** no log de eventos durante a sincronização de senha, verifique o guia de solução de problemas [PCNS relatando o erro 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Se a sincronização completa com o Agente de Gerenciamento de Serviço FIM for lenta, verifique a configuração de **crescimento automático** para TempDB, conforme descrito em [Solução de problemas de sincronização lenta ou total suspensa](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Se você estiver encontrando um erro de servidor parado com falha na criação por meio de serviços web usando o Agente de Gerenciamento de Serviços FIM, consulte [Informações de Suporte: falha na criação por meio de serviços web](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) para uma visão geral das causas.

