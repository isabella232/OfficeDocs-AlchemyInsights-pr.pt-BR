---
title: Configurar ponto de conexão de serviço (SCP)
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
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897407"
---
# <a name="configure-service-connection-point-scp"></a>Configurar ponto de conexão de serviço (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Motivo**: não é possível ler o objeto SCP e obter as informações do locatário do Azure AD
- **Resolução**: confira a seção [Configurar um ponto de conexão de serviço](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Plano de ação**

- Verifique se o dispositivo recebeu o GPO para a validação controlada.
- Verifique se o GPO criou as chaves do Registro.
- Certifique-se de ter 2 chaves criadas com seu ID de diretório e domínio onmicrosoft.

**Definir a configuração do Registro do lado do cliente para SCP**

Use o exemplo a seguir para criar um objeto de política de grupo (GPO) para implantar uma configuração de Registro que configure uma entrada SCP no Registro de seus dispositivos.

1. Abra um console de gerenciamento de política de grupo e crie um novo GPO em seu domínio.
     - Forneça um nome para o GPO recém-criado (por exemplo, ClientSideSCP)

2. Edite o GPO e localize o seguinte caminho: **Configuração do computador > Preferências > Configurações do Windows > Registro**.

3. Clique com o botão direito em **Registro** e selecione **Novo > Item do Registro**.

4. Na guia **Geral**, configure o seguinte:
  
- **Ação**: atualizar
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Caminho da chave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nome do valor**: TenantId
    
- **Tipo do valor**: REG_SZ
    
- **Dados do valor**: o GUID ou ID de diretório da instância do Azure AD (esse valor pode ser encontrado no **portal do Azure > Azure Active Directory > Propriedades > ID de diretório**)
 
- Clique em **OK**.
 
5. Clique com o botão direito em **Registro** e selecione **Novo > Item do Registro**.

6. Na guia **Geral**, configure o seguinte:
  
- **Ação**: atualizar
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Caminho da chave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nome do valor**: TenantName
    
- **Tipo do valor**: REG_SZ
    
- **Dados do valor**: o nome de domínio verificado se você estiver usando um ambiente federado, como AD FS. O nome de domínio verificado ou o nome de domínio onmicrosoft.com (por exemplo, contoso.onmicrosoft).com se você estiver usando um ambiente gerenciado

- Clique em **OK**.

7. Feche o editor do GPO recém-criado.

8. Vincule o GPO recém-criado à UO desejada contendo computadores associados ao domínio que pertencem ao seu conjunto de dados de distribuição controlado.

Para obter mais informações, confira [Validação controlada de associação híbrida do Azure AD - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) e [Solução de problemas de dispositivos híbridos associados ao Azure Active Directory | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









