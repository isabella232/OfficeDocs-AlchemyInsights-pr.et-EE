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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002116"
---
# <a name="error-attributevaluemustbeunique"></a>Tõrge: AttributeValueMustBeUnique

Tõrke AttributeValueMustBeUnique kõige levinum põhjus on kaks erineva SourceAnchoriga (immutableId) objekti, mille atribuudil ProxyAddresses ja/või UserPrincipalName on sama väärtus. Tõrke AttributeValueMustBeUnique parandamiseks:
  
1. Tuvastage dubleeritud proxyAddresses, userPrincipalName või muu atribuudi väärtus, mis vea põhjustab. Samuti saate tuvastada, millised kaks (või enam) objekti on konflikti kaasatud. Azure AD Ühendus Health for sync loodud aruanne aitab teil tuvastada kaks objekti.
    
2. Tuvastage, milline objekt peaks jätkuvalt dubleeritud väärtust omama ja millist objekti ei tohiks kasutada.
    
3. Eemaldage dubleeritud väärtus objektilt, mis ei tohiks seda väärtust omada. Pange tähele, et peaksite tegema muudatuse kataloogis, kust objekt on pärit. Mõnel juhul peate võib-olla ühe konfliktis oleva objekti kustutama.
    
4. Kui tegite muudatuse asutusesiseses AD-s, laske Azure AD-Ühendus azure AD-d sünkroonida, et viga parandatakse.
    

