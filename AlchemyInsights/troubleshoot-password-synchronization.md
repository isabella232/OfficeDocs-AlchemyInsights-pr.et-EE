---
title: Parooli sünkroonimise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732506"
---
# <a name="troubleshoot-password-synchronization"></a>Parooli sünkroonimise tõrkeotsing

Tõrkeotsing probleemidele, kus paroolid on sünkroonitud Azure AD ühenduse versiooni 1.1.614.0 või uuem versioon:
  
1. Avage uus Windows PowerShelli seansi Azure AD ühenduse serveris suvandi **Käivita administraatorina** .

2. Käivitage **Set-ExecutionPolicy Remoteallkirjastatud** või **seatud-ExecutionPolicy piiranguteta**.

3. Käivitage Azure AD ühenduse viisard.

4. Liikuge lehele **täiendavad tööülesanded** , valige **tõrkeotsing**ja klõpsake nuppu **edasi**.

5. Klõpsake lehel tõrkeotsing **käivitada PowerShelli tõrkeotsingu menüü käivitamiseks** .

6. Valige põhimenüüs **parooli sünkroonimise tõrkeotsing**.

7. Alammenüüs valige **parooli sünkroonimine ei tööta üldse**.

**Tõrkeotsinguülesande tulemuste mõistmine**
  
Tõrkeotsingu ülesanne teeb järgmised kontrollid:
  
- Valideerib, et parooli sünkroonimise funktsioon on lubatud Azure AD rentniku jaoks.

- Valideerib Azure AD ühenduse server ei ole vahekausta režiimis.

- Iga olemasoleva asutusesisese Active Directory konnektor (mis vastab olemasolevale Active Directory metsa):

- 
  - Valideerib, et parooli sünkroonimise funktsioon on lubatud.

  - Otsib parooli sünkroonimise südamelöögi sündmused Windowsi rakenduse sündmuselogid.

  - Iga Active Directory domeeni asutusesisese Active Directory konnektor:

  - Valideerib, et domeen on kättesaadav Azure AD ühenduse serverist.

  - Valideerib, et Active Directory domeeniteenused (AD DS) kontod, mida kasutatakse asutusesisese Active Directory konnektor on õige kasutajanimi, parool ja õigused parooli sünkroonimine.

Parooli sünkroonimise tõrkeotsingu kohta lisateabe saamiseks vaadake [tõrkeotsing parooli sünkroonimine AZURE AD ühenduse sünkroonimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  