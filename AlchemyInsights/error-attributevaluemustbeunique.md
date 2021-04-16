---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813756"
---
# <a name="error-attributevaluemustbeunique"></a>Tõrge: AttributeValueMustBeUnique

Tõrke AttributeValueMustBeUnique kõige levinum põhjus on kaks erineva SourceAnchoriga (immutableId) objekti, mille atribuudil ProxyAddresses ja/või UserPrincipalName on sama väärtus. Tõrke AttributeValueMustBeUnique parandamiseks:
  
1. Tuvastage dubleeritud proxyAddresses, userPrincipalName või muu atribuudi väärtus, mis vea põhjustab. Samuti saate tuvastada, millised kaks (või enam) objekti on konflikti kaasatud. Azure AD Connecti seisundi sünkroonimiseks loodud aruanne aitab teil tuvastada kaks objekti.
    
2. Tuvastage, milline objekt peaks jätkuvalt dubleeritud väärtust omama ja millist objekti ei tohiks kasutada.
    
3. Eemaldage dubleeritud väärtus objektilt, mis ei tohiks seda väärtust omada. Pange tähele, et peaksite tegema muudatuse kataloogis, kust objekt on pärit. Mõnel juhul peate võib-olla ühe konfliktis oleva objekti kustutama.
    
4. Kui tegite muudatuse kohapeal AD-s, laske Azure AD Connect'is tõrke muutmisel muudatust sünkroonida.
    

