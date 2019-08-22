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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526982"
---
# <a name="error-attributevaluemustbeunique"></a>Tõrge: AttributeValueMustBeUnique

AttributeValueMustBeUnique tõrke levinuim põhjus on kaks objekti koos erinevate SourceAnchor (immutableId) on sama väärtusega ProxyAddresses ja/või UserPrincipalName atribuudid. AttributeValueMustBeUnique vea parandamiseks:
  
1. Määrata dubleeritud proxyAddresses, userPrincipalName või muu atribuudi väärtus, mis tõrget põhjustab. Ka kindlaks, millised kahe (või enama) objektid on seotud konflikti. Aruanne loodud Azure AD ühenduse tervise sünkroonimise saate tuvastada kaks objekti.
    
2. Kindlaks teha, milline objekt peaks jätkuvalt olema dubleeritud väärtust ja milline objekt ei tohiks.
    
3. Eemaldage dubleeritud väärtust objekti, mis ei peaks seda väärtust. Pange tähele, et peate kataloogi, kui objekt on pärit muutus. Mõnel juhul peate kustutada ühe objekti konfliktis.
    
4. Kui tegite muutuse kohta ruumides, AD, lase Azure AD ühenduse viga saada fikseeritud muutuste sünkroonimine.
    

