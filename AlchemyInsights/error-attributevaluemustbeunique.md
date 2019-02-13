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
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916520"
---
# <a name="error-attributevaluemustbeunique"></a>Tõrge: AttributeValueMustBeUnique

AttributeValueMustBeUnique tõrke levinuim põhjus on kaks objekti koos erinevate SourceAnchor (immutableId) on sama väärtusega ProxyAddresses ja/või UserPrincipalName atribuudid. AttributeValueMustBeUnique vea parandamiseks:
  
1. Määrata dubleeritud proxyAddresses, userPrincipalName või muu atribuudi väärtus, mis tõrget põhjustab. Ka kindlaks, millised kahe (või enama) objektid on seotud konflikti. Aruanne loodud Azure AD ühenduse tervise sünkroonimise saate tuvastada kaks objekti.
    
2. Kindlaks teha, milline objekt peaks jätkuvalt olema dubleeritud väärtust ja milline objekt ei tohiks.
    
3. Eemaldage dubleeritud väärtust objekti, mis ei peaks seda väärtust. Pange tähele, et peate kataloogi, kui objekt on pärit muutus. Mõnel juhul peate kustutada ühe objekti konfliktis.
    
4. Kui tegite muutuse kohta ruumides, AD, lase Azure AD ühenduse viga saada fikseeritud muutuste sünkroonimine.
    

