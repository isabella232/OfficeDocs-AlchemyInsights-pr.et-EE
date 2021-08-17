---
title: ConsistencyGuid / sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044336"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

Azure AD Ühendus (versioon 1.1.524.0 ja pärast) hõlbustab nüüd msDS-ConsistencyGuidi kasutamist atribuudi sourceAnchorna. Selle funktsiooni kasutamisel konfigureerib Azure AD Ühendus sünkroonimisreeglid automaatselt:
  
- Kasutage atribuuti msDS-ConsistencyGuid user-objektide atribuudina sourceAnchor. ObjectGUID-d kasutatakse muude objektitüüpide jaoks.
    
- Azure AD Ühendus kirjutab iga asutusesisese AD kasutaja objekti, mille atribuut msDS-ConsistencyGuid pole asustatud, tagasi asutusesisese Active Directory atribuudile msDS-ConsistencyGuid. Kui atribuut msDS-ConsistencyGuid on asustatud, ekspordib Azure AD Ühendus objekti Azure AD-sse.
    
 **Märkus.** Kui kohapealne AD-objekt on imporditud Azure AD Ühendus (st imporditud AD Connectori ruumi ja prognoositud metaversumisse), ei saa te selle sourceAnchori väärtust enam muuta. Antud asutusesisese AD-objekti atribuudi sourceAnchor määramiseks konfigureerige selle atribuut msDS-ConsistencyGuid enne selle importimist Azure AD Ühendus. 
  
Lisateavet SourceAnchori ja ConsistencyGuid kohta leiate järgmistest artiklitest: [Azure AD Ühendus: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

