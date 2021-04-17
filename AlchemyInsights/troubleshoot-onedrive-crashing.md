---
title: Solução de problemas do OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826187"
---
# <a name="troubleshoot-onedrive-crashes"></a>Solução de problemas do OneDrive

Se o OneDrive falhar repetidamente, experimente estas etapas de solução de problemas:

**Garantir que as chaves do registro não estejam definidas:**

1. Usando o Editor de Registro, navegue até HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Se DisableFileSyncNGSC estiver presente e definido como 1, abra a chave e altere o valor para 0.
3. Inicie o OneDrive manualmente acessando Iniciar ![Pressione a tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), digite OneDrive na caixa de pesquisa e, em seguida, clique no aplicativo da área de trabalho do OneDrive.

**Redefinir o OneDrive:**

Observações:

- Redefinir o OneDrive desconectará todas as conexões de sincronização existentes (inclusive seu OneDrive pessoal, caso esteja configurado).
- Você não perde dados ou arquivos ao redefinir o OneDrive no seu computador.

**Para redefinir o OneDrive:**

1. Abra uma caixa de diálogo Executar pressionando a tecla Windows e R.
2. Digite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset e pressione OK. Uma janela de Comando pode aparecer durante breves instantes.
3. Inicie o OneDrive manualmente acessando Iniciar ![Pressione a tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), digite OneDrive na caixa de pesquisa e, em seguida, clique no aplicativo da área de trabalho do OneDrive.

Observações:

- Se você escolhido sincronizar apenas algumas pastas antes da redefinição, precisará fazer isso novamente após concluir a sincronização. Leia  [Escolher quais pastas do OneDrive sincronizar com seu computador](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  para mais informações.
- Será necessário concluir isso para o seu OneDrive pessoal e para o OneDrive for Business.