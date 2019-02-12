---
title: Parooli sünkroonimise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924692"
---
# <a name="troubleshoot-password-synchronization"></a>Parooli sünkroonimise tõrkeotsing

Tõrkeotsingu, kus puuduvad paroolid on sünkroonitud Azure AD ühenduse versioon 1.1.614.0 või uuem versioon:
  
1. Avage uus Windows PowerShelli seanss Azure AD ühenduse serveri suvandiga **Käivita administraatorina** . 
    
2. Käivitage **Set-ExecutionPolicy RemoteSigned** või **Set-ExecutionPolicy piiramatu**. 
    
3. Azure AD ühenduse viisardit käivitada.
    
4. Liikuge selle ** lisaülesandeid ** avamiseks valige ** tõrkeotsing **, ja klõpsake nuppu **edasi**. 
    
5. Klõpsake lehel tõrkeotsing **käivitada tõrkeotsingu käivitamiseks** menüü PowerShelli. 
    
6. Peamenüüst valige **Parooli sünkroonimise tõrkeotsing**. 
    
7. Alammenüü, valige **parool ei tööta üldse**. 
    
 **Arusaamiseks tõrkeotsingu ülesanne**
  
Tõrkeotsingu toiming teeb järgmised kontrollid:
  
- Kinnitab, et parooli sünkroonimise funktsiooni on lubatud Azure AD üürnikule.
    
- Kinnitab, et Azure AD ühenduse server ei ole lavastus režiimis.
    
- Jaoks iga olemasoleva asutusesisese Active Directory konnektor (mis vastab olemasolevaid Active Directory metsa):
    
- 
  - Kinnitab, et parooli sünkroonimise funktsioon on lubatud.
    
  - Otsib parooli sünkroonimise pulss sündmused Windowsi rakenduste sündmuste logisse.
    
  - Iga Active Directory domeeni all asutusesisese Active Directory konnektor:
    
  - Kinnitab, et on kättesaadav Azure AD ühenduse server.
    
  - Kinnitab, et Active Directory Domain Services (AD DS) kontosid, mida asutusesisese Active Directory konnektor on õige kasutajanimi, parool ja parooli sünkroonimine vajalikud õigused.
    
Rohkem tõrkeotsing parooli sünkroonimise kohta vaadake teemast [tõrkeotsing parooli sünkroonimine Azure AD ühenduse sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

