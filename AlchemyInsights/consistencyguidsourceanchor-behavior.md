---
title: ConsistencyGuid / sourceAnchor käitumine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498514"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor käitumine

Azure AD ühenduse loomine (versioon 1.1.524.0 ja pärast) nüüd lihtsustab kasutamist msDS-ConsistencyGuid kui sourceAnchor atribuut. Kui kasutate seda funktsiooni, Azure AD ühenduse konfigureerib automaatselt sünkroonimise reeglid:
  
- Kasutada msDS-ConsistencyGuid sourceAnchor atribuut kasutaja objektid. FederatedIdentity kasutatakse muud objekti tüüpi.
    
- Ühegi esitatud asutusesisese AD kasutaja objekti kelle vaevuste ConsistencyGuid atribuut ei sisestata, Azure AD ühenduse kirjutab oma FederatedIdentity väärtusena vaevuste ConsistencyGuid atribuut asutusesisese Active Directory. Pärast vaevuste ConsistencyGuid atribuut on asustatud, Azure AD ühenduse siis ekspordib objekti Azure AD.
    
 **Märkus:** Kui asutusesisese AD objekti imporditakse Azure AD ühenduse (st imporditud AD konnektori ruumi ja metaversumi viia), selle sourceAnchor väärtuseks ei saa enam muuta. Täpsustada sourceAnchor väärtus on esitatud asutusesisese AD objekti, konfigureerima oma vaevuste ConsistencyGuid atribuut see imporditakse Azure AD ühenduse. 
  
SourceAnchor ja ConsistencyGuid kohta lisateabe saamiseks vaadake järgmist: [Azure AD ühenduse: kujundada mõisted](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

