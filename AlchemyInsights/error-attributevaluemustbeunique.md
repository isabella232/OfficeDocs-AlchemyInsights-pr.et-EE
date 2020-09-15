---
title: AttributeValueMustBeUnique tõrge
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709147"
---
# <a name="error-attributevaluemustbeunique"></a>Tõrge: AttributeValueMustBeUnique

AttributeValueMustBeUnique ' i tõrke kõige tavalisem põhjus on kaks erinevat SourceAnchor (immutableId) objekti, millel on ProxyAddresses ja/või UserPrincipalName atribuudid sama väärtus. AttributeValueMustBeUnique vea parandamiseks tehke järgmist.
  
1. Tuvastage viga põhjustava dubleeritud proxyAddresses, userPrincipalName või muu atribuudi väärtus. Samuti saate tuvastada, millised kaks (või enam) objekti on konfliktis kaasatud. Azure AD Connecti Health for Synci loodud aruanded aitavad teil kaks objekti tuvastada.
    
2. Tuvastage, millisel objektil peaks jätkuma dubleeritud väärtus ja mida objekt ei peaks olema.
    
3. Eemaldage sellelt objektilt kopeeritud väärtus, mis ei tohiks olla selle väärtusega. Pange tähele, et peate tegema muudatuse kataloogist, kust objekt pärineb. Mõnel juhul peate võib-olla mõne konfliktis oleva objekti kustutama.
    
4. Kui tegite kohapealses REKLAAMIs muudatuse, siis lubage Azure AD Connecti abil taastada tõrke muutus.
    

