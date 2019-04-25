---
title: ConsistencyGuid / sourceAnchor käitumine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408104"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor käitumine

Azure AD ühenduse loomine (versioon 1.1.524.0 ja pärast) nüüd lihtsustab kasutamist msDS-ConsistencyGuid kui sourceAnchor atribuut. Kui kasutate seda funktsiooni, Azure AD ühenduse konfigureerib automaatselt sünkroonimise reeglid:
  
- Kasutada msDS-ConsistencyGuid sourceAnchor atribuut kasutaja objektid. FederatedIdentity kasutatakse muud objekti tüüpi.
    
- Ühegi esitatud asutusesisese AD kasutaja objekti kelle vaevuste ConsistencyGuid atribuut ei sisestata, Azure AD ühenduse kirjutab oma FederatedIdentity väärtusena vaevuste ConsistencyGuid atribuut asutusesisese Active Directory. Pärast vaevuste ConsistencyGuid atribuut on asustatud, Azure AD ühenduse siis ekspordib objekti Azure AD.
    
 **Märkus:** Kui asutusesisese AD objekti imporditakse Azure AD ühenduse (st imporditud AD konnektori ruumi ja metaversumi viia), selle sourceAnchor väärtuseks ei saa enam muuta. Täpsustada sourceAnchor väärtus on esitatud asutusesisese AD objekti, konfigureerima oma vaevuste ConsistencyGuid atribuut see imporditakse Azure AD ühenduse. 
  
SourceAnchor ja ConsistencyGuid kohta lisateabe saamiseks vaadake järgmist: [Azure AD ühenduse: kujundada mõisted](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

