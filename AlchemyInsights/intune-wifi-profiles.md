---
title: Perfis Wi-Fi do Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509037"
---
# <a name="intune-wi-fi-profiles"></a>Perfis Wi-Fi do Intune

A implementação bem sucedida da conectividade Wi-Fi para clientes MDM depende de um perfil corretamente implantado que reflita as exigências da infraestrutura de Wi-Fi corporativa. Para rever as configurações apropriadas das plataformas do cliente que você está investigando, consulte: 

[Adicionar configurações Wi-Fi aos dispositivos com Android no Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Adicionar configurações Wi-Fi aos dispositivos dedicados e totalmente gerenciados do Android Enterprise no Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Adicionar configurações Wi-Fi aos dispositivos iOS e iPadOS no Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Adicionar configurações Wi-Fi ao Windows 10 e dispositivos posteriores no Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importar configurações Wi-Fi aos dispositivos Windows no Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Problemas comuns**

**Estou implantando um perfil de Wi-Fi que depende de um certificado de implantação especificado no perfil de Wi-Fi. Entretanto, os perfis de configuração estão exibindo um status de erro.**

Verifique se o seu dispositivo recebeu o certificado.

1. No Intune, acesse **Todos os dispositivos** e selecione o dispositivo > **Configuração do dispositivo**.

2. Verifique se todos os perfis esperados estão listados e em um estado bem-sucedido.

3. Quanto a um perfil do Android, se você tiver certificados intermediários na sua cadeia de certificados, certifique-se de que eles sejam implantados nos dispositivos Android.

    Para verificar o status do certificado, acesse **Configuração do dispositivo** > **Perfis** > **AC intermediário do Android** > **Propriedades** > **Certificado de confiança**.

Se você continuar a visualizar erros, reveja os procedimentos e as seções de solução de problemas. Para obter mais informações, consulte [Visão geral da solução de problemas dos perfis de certificados SCEP com o Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Eu implantei um perfil de Wi-Fi em um dispositivo. O Intune está mostrando que foi bem sucedido, mas o dispositivo não está se conectando ao Wi-Fi.**

Um status de sucesso significa que o Intune implantou com sucesso o perfil conforme configurado. Entretanto, talvez essas configurações não correspondam aos requisitos de sua rede e/ou autenticação. Para obter mais detalhes sobre a tentativa de conexão, revise os logs na infraestrutura e no serviço de autenticação (no controlador do ponto de acesso de Wi-Fi e no servidor NPS/Radius). Talvez você tenha que trabalhar com sua equipe de infraestrutura de rede ou com o fornecedor de Wi-Fi de terceiros para reunir e revisar os logs.