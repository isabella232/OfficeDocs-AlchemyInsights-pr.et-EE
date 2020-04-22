---
title: Tõrge AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703170"
---
# <a name="error-attributevaluemustbeunique"></a>Tõrge: AttributeValueMustBeUnique

Kõige tavalisem põhjus AttributeValueMustBeUnique tõrge on kaks objekti, millel on erinevad SourceAnchor (immutableId) on sama väärtus ProxyAddresses ja/või UserPrincipalName atribuute. AttributeValueMustBeUnique tõrke parandamiseks:
  
1. Nimetage dubleeritud proxyAddresses, userPrincipalName või muud atribuudi väärtus, mis põhjustab tõrke. Samuti saate tuvastada, millised kaks (või enam) objekti on konfliktis kaasatud. Azure AD ühenduse tervise sünkroonimise loodud aruanne aitab teil tuvastada kaks objekti.
    
2. Tuvastage, milline objekt peaks jätkuvalt olema dubleeritud väärtus ja millist objekti ei tohiks.
    
3. Eemaldage dubleeritud väärtus objekti, mis peaks olema see väärtus. Pange tähele, et peaksite muutma kataloogi, kust objekt pärineb. Mõnel juhul peate võib-olla kustutama ühe objektist konfliktis.
    
4. Kui tegite asutusesisese AD muudatuse, lubage Azure AD ühenduse sünkroonimise tõrke muudatuse saada fikseeritud.
    

