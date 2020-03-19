---
title: Catchall do tema do Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2605"
- "9000701"
ms.openlocfilehash: c7f7e14b17b51b916b7acb4a485eaed07f5be53b
ms.sourcegitcommit: 45b50760c00b5639b7199cb3812e44404ba04695
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42744992"
---
# <a name="teams-common-issues-and-resolutions"></a>Problemas e resoluções comuns do Teams

Para uma resposta mais específica, tente reformular a sua pergunta para incluir os erros que você está encontrando ou os recurso do Teams que você está usando.

Se você precisar de ajuda para implantar o Teams para dar suporte a funcionários remotos (WFH), devido à COVID-19, revise [Dar suporte a funcionários remotos usando o Microsoft Teams](https://docs.microsoft.com/microsoftteams/support-remote-work-with-teams). Além disso, você pode estar qualificado para obter assistência na implantação do programa Microsoft 365 FastTrack: visite o [Centro FastTrack](https://www.microsoft.com/fasttrack) para enviar uma solicitação.

Para todos os clientes do Teams:

- **Novo usuário do Teams?** Confira [Introdução ao Microsoft Teams](https://docs.microsoft.com/microsoftteams/get-started-with-teams-quick-start).
- **Habilite o acesso para convidado do Teams:** Confira a [lista de verificação de acesso para convidado do Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) e verifique se todas as etapas foram concluídas. Recursos adicionais:
    - [Entendendo o Acesso para Convidados no Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Configuração – Lista de Verificação de Acesso de Convidados do Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Como um convidado ingressa em uma equipe](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Reuniões e Discagem no Teams**: precisa de ajuda para ativar ou configurar audioconferências no Microsoft Teams? Esse usuário foi criado recentemente? Em caso afirmativo, você precisará esperar de 2 a 24 horas **para que as configurações sejam efetivadas**. 

    Para verificar se o usuário está licenciado para conferências de áudio e tem um número de chamada padrão:
    1.    Vá para Usuários ativos e selecione o usuário em questão.
    2.    Dependendo da versão do centro de administração, escolha Licenças e Aplicativos ou clique em Editar em Licenças do produto.
    3.    Confirme se o usuário tem licenças selecionadas para Audioconferência, Microsoft Teams e para o Skype for Business Online (plano 2).
    4.    Em Centro de Administração de Usuários, clique em Mostrar todos e em Teams.
    5.    No centro de administração do Microsoft Teams, clique em Portal herdado.
    6.    No centro de administração do Skype for Business, clique em audioconferência e, em seguida, em usuários.
    7.    Selecione o usuário em questão e verifique se o usuário tem um Número de Chamada Padrão Tarifada.
    
    Para saber mais, confira [Planos de chamadas do Office 365](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) ou ligue para a equipe de cobrança do Microsoft Commerce para obter ajuda com perguntas relacionadas a licenciamento.

    Recursos adicionais:

    - [Conferências e reuniões no Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audioconferência no Office 365](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Licença do Teams Exploratory**: a experiência do Microsoft Teams Exploratory permite que os usuários de sua organização que tenham o Azure Active Directory (AAD) e não estejam licenciados para o Teams iniciem uma experiência exploratória do Teams. Os administradores podem ativar ou desativar esse recurso para os usuários em sua organização. O [Microsoft Commercial Cloud Trial](https://docs.microsoft.com/microsoftteams/iw-trial-teams) anterior agora foi substituído pela experiência do Teams Exploratory.

    Recursos adicionais:

    - [Como os usuários se inscrevem na experiência do Teams Exploratory](https://docs.microsoft.com/microsoftteams/teams-exploratory#how-users-sign-up-for-the-teams-exploratory-experience)
    - [Gerenciar a experiência do Teams Exploratory](https://docs.microsoft.com/microsoftteams/teams-exploratory#manage-the-teams-exploratory-experience)

- **Canais Privados**: os Canais Privados do Microsoft Teams criam espaços concentrados na colaboração com suas equipes. O acesso é restrito aos usuários da equipe que forem proprietários ou membros do canal privado. É possível adicionar qualquer pessoa, inclusive convidados, como membro de um canal privado, desde que já sejam membros da equipe.

    Você pode usar o canal privado para limitar a colaboração àqueles que precisam de conhecimento ou se quiser facilitar a comunicação entre um grupo de pessoas atribuídas para um projeto específico, sem ter que criar uma equipe adicional para gerenciar.

    Recursos adicionais:
    - [Criação e associação a canal privado](https://docs.microsoft.com/microsoftteams/private-channels#private-channel-creation-and-membership)
    - [Gerenciar configurações e associação a canal privado](https://docs.microsoft.com/microsoftteams/private-channels#manage-private-channel-membership-and-settings)

- **Políticas de Reuniões**: são usadas para controlar os recursos disponibilizados para os participantes de reunião programada pelos usuários de sua organização. Depois de criar uma política e fazer suas alterações, você pode atribuir usuários à política. 
    - **Alterar ou criar uma política de reunião**: para isso, acesse o **centro de administração do Microsoft Teams > Reuniões > Políticas de reunião**. Selecione uma política na lista ou clique em Adicionar. Se você estiver criando uma nova política, adicione um nome e uma descrição. O nome não pode conter caracteres especiais ou ter mais de 64 caracteres. Escolha as configurações e clique em **Salvar**.

        Por exemplo, digamos que você tenha um grupo de usuários e queira limitar a quantidade de largura de banda que a reunião exigiria. Você criaria uma nova política personalizada chamada "Largura de banda limitada" e desativaria as seguintes configurações:

        Em **Áudio e vídeo**:
        - Desative a opção Permitir gravação na nuvem.
        - Desative a opção Permitir vídeo IP.

        Em **Compartilhamento de conteúdo**:
        - Desative o modo de compartilhamento de tela.
        - Desative a opção Permitir quadro de comunicações.
        - Desative a opção Permitir anotações compartilhadas.

        Em seguida, atribua a política aos usuários.

- **Atribuir uma política de reunião aos usuários**

    1. Na barra de navegação à esquerda do centro de administração do Microsoft Teams, vá para **Usuários** e clique no usuário.
    2. Selecione o usuário clicando à esquerda do nome de exibição do usuário e clique em **Editar configurações**.
    3. Em **Política de reunião**, selecione a política que você deseja atribuir e clique em **Aplicar**.

    Para atribuir uma política a vários usuários de uma só vez, confira [Editar as configurações de usuários do Teams em massa](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk). Ou você pode fazer o seguinte:

    1. Na barra de navegação à esquerda do centro de administração do Microsoft Teams, vá para **Reuniões > Políticas de Reunião**.
    2. Escolha a política clicando à esquerda do nome da política.
    3. Selecione **Gerenciar usuários**.
    4. No painel **Gerenciar usuários**, procure o usuário pelo nome de exibição ou pelo nome de usuário, escolha o nome e clique em **Adicionar**. Repita esta etapa para cada usuário que você deseja adicionar.
    5. Depois de terminar de adicionar as colunas, clique em **Salvar**.

- **Solucionar um problema de teclado de discagem ausente:**  

    - Certifique-se de que o usuário recebeu uma [licença do Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Verifique se o usuário possui um [Plano de Chamadas](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) atribuído.
    - Habilite os usuários para o [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Solucionar problemas de entrada do Teams:** Primeiro, verifique se o [serviço do Microsoft Teams está íntegro](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Em seguida, verifique se há códigos de erro comuns e confira [Por que estou tendo problemas para entrar no Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)  Você também pode precisar revisar os [Modelos de identidade e a autenticação no Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).

**Para os clientes do Education:**

Se os usuários estiverem vendo a mensagem "você não sabe o que está perdendo!" Lembre-se de [Habilitar o Microsoft Teams para a sua escola](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Em locatários EDU, o Microsoft Teams não está habilitado por padrão. será preciso ativá-lo primeiro.

Em seguida, confira [Ensino remoto e aprendizagem no Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) para saber quais são as orientações mais atualizadas sobre como configurar a sua escola, planejar a lição, atender virtualmente e compartilhar conteúdo com os alunos.

Por fim, lembre-se de conferir os slides e os vídeos de treinamento dos administradores de TI do Microsoft Teams e muito mais aqui: https://docs.microsoft.com/MicrosoftTeams/itadmin-readiness#technical-training. 
