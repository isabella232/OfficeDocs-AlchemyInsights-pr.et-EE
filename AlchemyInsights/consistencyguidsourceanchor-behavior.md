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
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816988"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

Azure AD Connect (versioon 1.1.524.0 ja pärast seda) hõlbustab nüüd msDS-ConsistencyGuidi kasutamist atribuudi sourceAnchorna. Selle funktsiooni kasutamisel konfigureerib Azure AD Connect sünkroonimisreeglid automaatselt:
  
- Kasutage atribuuti msDS-ConsistencyGuid user-objektide atribuudina sourceAnchor. ObjectGUID-d kasutatakse muude objektitüüpide jaoks.
    
- Mis tahes asutusesisese AD-kasutaja objekti puhul, mille atribuut msDS-ConsistencyGuid pole asustatud, kirjutab Azure AD Connect oma objektiGUID-väärtuse tagasi asutusesisese Active Directory atribuudile msDS-ConsistencyGuid. Kui atribuut msDS-ConsistencyGuid on asustatud, ekspordib Azure AD Connect objekti Azure AD-sse.
    
 **Märkus.** Kui kohapealne AD-objekt on azure AD Connecti imporditud (st imporditud AD Connectori ruumi ja prognoositud metaversumisse), ei saa te selle sourceAnchori väärtust enam muuta. Antud asutusesisese AD-objekti atribuudi sourceAnchor määramiseks konfigureerige selle atribuut msDS-ConsistencyGuid enne selle importimist Azure AD Connecti. 
  
Lisateavet SourceAnchori ja ConsistencyGuid kohta leiate järgmistest artiklitest: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

