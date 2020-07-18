---
title: Problema ao abrir ou baixar arquivos no Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146745"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problema ao abrir ou baixar arquivos no Yammer

O Yammer clássico tem suporte para várias opções de carregamentos de arquivos para mensagens e grupos. Dependendo da configuração de rede, arquivos são armazenados no SharePoint por regra.

O seletor de arquivos no novo Yammer ainda não tem suporte para todas as opções disponíveis no Yammer clássico. Uma atualização futura adicionará novos recursos. Para saber mais, confira [Anexar um arquivo ou imagem a uma conversa no Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Não é possível abrir ou baixar um arquivo**  

Um arquivo pode ser carregado no Yammer mas também ser vinculado a um arquivo no SharePoint Online. Para solucionar esse problema, primeiro você precisa determinar o local desse arquivo. Se o arquivo tiver sido carregado no Yammer, ele terá uma URL *. yammer.com. Verifique que os URLs e os endereços de IP necessários estão desbloqueados. Para saber mais, confira o post do blog[Usando endereços de IP embutidos no Yammer não é recomendável](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Verifique se um usuário que também é um administrador global pode baixar o arquivo. Se o arquivo for privado, talvez seja necessário usar o modo de conteúdo particular. Para saber mais, confira [Monitorar conteúdo particular no Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Convidados no nível da rede do Yammer e arquivos no SharePoint Online**  

[Os convidados no nível da rede no Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) não usam o Azure AD B2B e são internos do serviço Yammer, portanto, não podem acessar arquivos do Yammer armazenados no SharePoint. Crie um usuário AAD B2B que possa acessar documentos na biblioteca no SharePoint Online usando essa identidade. Para obter informações sobre o futuro suporte a clientes B2B do Azure AD no Yammer, confira [suporte para Convidados B2B (Business-to-Business) na visualização do Yammer - Termos e perguntas frequentes](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).