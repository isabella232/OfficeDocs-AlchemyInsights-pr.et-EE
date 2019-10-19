---
title: Tõrge AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36526982"
---
# <a name="error-attributevaluemustbeunique"></a>Tõrge: AttributeValueMustBeUnique

Kõige tavalisem põhjus AttributeValueMustBeUnique tõrge on kaks objekti, millel on erinevad SourceAnchor (immutableId) on sama väärtus ProxyAddresses ja/või UserPrincipalName atribuute. AttributeValueMustBeUnique tõrke parandamiseks:
  
1. Nimetage dubleeritud proxyAddresses, userPrincipalName või muud atribuudi väärtus, mis põhjustab tõrke. Samuti saate tuvastada, millised kaks (või enam) objekti on konfliktis kaasatud. Azure AD ühenduse tervise sünkroonimise loodud aruanne aitab teil tuvastada kaks objekti.
    
2. Tuvastage, milline objekt peaks jätkuvalt olema dubleeritud väärtus ja millist objekti ei tohiks.
    
3. Eemaldage dubleeritud väärtus objekti, mis peaks olema see väärtus. Pange tähele, et peaksite muutma kataloogi, kust objekt pärineb. Mõnel juhul peate võib-olla kustutama ühe objektist konfliktis.
    
4. Kui tegite asutusesisese AD muudatuse, lubage Azure AD ühenduse sünkroonimise tõrke muudatuse saada fikseeritud.
    

