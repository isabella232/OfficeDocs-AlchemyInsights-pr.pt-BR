---
title: Trabalhando com as Bibliotecas de Autenticação
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: b667e699e1595b21d80788123de13daffbe79a35b1671e9d35eaa6cd980693db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083074"
---
# <a name="working-with-authentication-libraries"></a>Trabalhando com as Bibliotecas de Autenticação

Para resolver o problema da MSAL (Biblioteca de Autenticação Microsoft), execute as seguintes etapas recomendadas:

1. **Trabalhando com a MSAL**: [Bibliotecas de Autenticação da plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - Este artigo mostra o suporte da Biblioteca de Autenticação da Microsoft para vários tipos de aplicativo. Ele inclui links para o código-fonte da biblioteca; onde obter o pacote do projeto do seu aplicativo; e se a biblioteca dá suporte à entrada do usuário (autenticação), acesso a APIs da Web protegidas (autorização) ou a ambos.

2. **Autenticação da Solução de Problemas**: A MSAL oferece suporte a vários fluxos para uso em diferentes cenários de aplicativos. Dependendo de como o aplicativo cliente foi criado, a MSAL pode usar um ou mais fluxos de autenticação com suporte na plataforma de identidade da Microsoft. Esses fluxos podem produzir vários tipos de tokens e códigos de autorização e exigem tokens diferentes para que eles funcionem.

3. **Tokens de Acesso**: [Token de acesso da plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Saiba como sua API pode validar e usar as declarações dentro de um token de acesso. Toda a documentação nesse artigo, exceto quando indicado, aplica-se somente aos tokens emitidos para APIs que você registrou. Isso não se aplica aos tokens emitidos para APIs de propriedade da Microsoft; nem podem ser usados para validar como a plataforma de identidade da Microsoft emitirá tokens para uma API que você cria.

**Fim do suporte à Biblioteca de Autenticação do Azure Active Directory (ADAL)**

- **A partir de 30 de junho de 2020,** não adicionaremos mais nenhum novo recurso à ADAL e ao Azure AD Graph. Continuaremos fornecendo suporte técnico e atualizações de segurança, mas não forneceremos mais atualizações de recursos.
- **A partir de 30 de junho de 2022,** encerraremos o suporte à ADAL e ao Azure AD Graph, e não forneceremos mais suporte técnico ou atualizações de segurança.
- Os aplicativos que usam a ADAL nas versões existentes do Sistema Operacional continuarão a funcionar após esse período, mas não *receberão nenhum suporte técnico ou atualizações de segurança*.
- Os aplicativos que usam o Azure AD Graph após esse período, podem não receber mais respostas do ponto de extremidade do Azure AD Graph.

**Migração da ADAL**

- Recomendamos a atualização para a MSAL, que tem os últimos recursos e as atualizações de segurança.
- Se você estiver usando aplicativos da Microsoft, saiba que a Microsoft está no processo de migração de seus aplicativos para o MSAL até a data limite do fim do suporte, garantindo que eles se beneficiarão dos aperfeiçoamentos de recursos e segurança contínuos da MSAL.

1. [Leia as perguntas frequentes sobre a ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Saiba mais sobre como migrar aplicativos por plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Se, depois de ler o guia para a plataforma do seu aplicativo, você tiver mais perguntas poderá postar no [Perguntas e Respostas da Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) com a marca [azure-ad-adal-deprecation] ou abrir um problema no repositório GitHub da biblioteca. Consulte a seção [Idiomas e Estruturas](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) do artigo **Visão Geral da MSAL** para links para o repositório de cada biblioteca.
4. **Se precisar de ajuda para entender qual de seus aplicativos usa a ADAL**, recomendamos que você reveja todos o códigos-fonte dos aplicativos. Se aplicável, entre em contato com qualquer provedor de software independente (ISVs) ou provedores de aplicativo. O suporte da Microsoft também pode fornecer uma lista de todos os aplicativos da ADAL que não são da Microsoft em seu locatário.







