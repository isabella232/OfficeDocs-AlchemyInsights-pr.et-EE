---
title: ConsistencyGuid/sourceAnchor käitumine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705729"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor käitumine

Azure AD ühenduse (versioon 1.1.524.0 ja pärast) nüüd hõlbustab msDS-ConsistencyGuid kasutamine sourceAnchor atribuut. Selle funktsiooni kasutamisel konfigureerib Azure AD Connect automaatselt sünkroonimisreeglid:
  
- Kasutage msDS-ConsistencyGuid kui sourceAnchor atribuut kasutaja objektid. ObjectGUID-i kasutatakse muude objektitüüpide puhul.
    
- Iga asutusesisese AD kasutaja objekti, mille msDS-ConsistencyGuid atribuut ei ole asustatud, Azure AD ühenduse kirjutab oma objectGUID väärtus tagasi on asutusesisese Active Directory atribuudi msDS-ConsistencyGuid. Pärast msDS-ConsistencyGuid atribuut on asustatud Azure AD ühenduse seejärel eksportida objekti Azure AD.
    
 **Märkus:** Kui asutusesisese AD objekti imporditakse Azure AD ühenduse (st imporditud AD connector Space ja prognoositud Metaverse), ei saa muuta selle sourceAnchor väärtus enam. Konkreetse asutusesisese AD objekti sourceAnchor väärtuse määramiseks Konfigureerige selle msDS-ConsistencyGuid atribuut enne importimist Azure AD ühenduse. 
  
SourceAnchor ja ConsistencyGuid kohta lisateabe saamiseks vaadake järgmist: [AZURE AD ühenduse: kujunduse mõisted](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

