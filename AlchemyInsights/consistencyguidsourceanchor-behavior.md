---
title: ConsistencyGuid/sourceAnchor käitumine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756279"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor käitumine

Azure AD Connect (versioon 1.1.524.0 ja After) hõlbustab nüüd luu-ja lihaskonna vaevuste-ConsistencyGuid kasutamist kui sourceAnchor atribuuti. Selle funktsiooni kasutamisel konfigureerib Azure AD Connect automaatselt sünkroonimise reeglid.
  
- Kasutage luu-ja lihaskonna vaevusi – ConsistencyGuid sourceAnchor atribuuti. ObjectGUID kasutatakse muud tüüpi objektide puhul.
    
- Kui kohapealne AD kasutaja objekt, mille luu-ja lihaskonna vaevuse-ConsistencyGuid atribuut pole asustatud, kirjutab Azure AD Connect selle objectGUID väärtuseks tagasi kohapealses Active Directorys asuvasse luu-ja lihaskonna vaevuste-ConsistencyGuid atribuuti. Pärast seda, kui luu-ja lihaskonna vaevusi-ConsistencyGuid atribuut on asustatud, eksporditakse Azure AD ja seejärel eksporditakse objekt Azure AD
    
 **Märkus:** Kui kohapealne AD objekt imporditakse Azure AD Connect (see tähendab, et see on imporditud AD Connectori ruumi ja kavandatakse metaversumi), ei saa te selle sourceAnchor enam muuta. Antud kohapealse reklaami objekti sourceAnchor määramiseks Konfigureerige selle luu-ja lihaskonna vaevuste-ConsistencyGuid atribuut, enne kui see imporditakse Azure AD Connecti. 
  
Lisateavet SourceAnchor ja ConsistencyGuid kohta leiate järgmistest teemadest: [AZURE ad Connect: kujunduse kontseptsioonid](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

