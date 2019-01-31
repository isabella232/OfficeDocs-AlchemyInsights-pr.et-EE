---
title: ConsistencyGuid / sourceAnchor käitumine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659587"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="2d142-102">ConsistencyGuid / sourceAnchor käitumine</span><span class="sxs-lookup"><span data-stu-id="2d142-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="2d142-p101">Azure AD ühenduse loomine (versioon 1.1.524.0 ja pärast) nüüd lihtsustab kasutamist msDS-ConsistencyGuid kui sourceAnchor atribuut. Kui kasutate seda funktsiooni, Azure AD ühenduse konfigureerib automaatselt sünkroonimise reeglid:</span><span class="sxs-lookup"><span data-stu-id="2d142-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="2d142-p102">Kasutada msDS-ConsistencyGuid sourceAnchor atribuut kasutaja objektid. FederatedIdentity kasutatakse muud objekti tüüpi.</span><span class="sxs-lookup"><span data-stu-id="2d142-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="2d142-p103">Ühegi esitatud asutusesisese AD kasutaja objekti kelle vaevuste ConsistencyGuid atribuut ei sisestata, Azure AD ühenduse kirjutab oma FederatedIdentity väärtusena vaevuste ConsistencyGuid atribuut asutusesisese Active Directory. Pärast vaevuste ConsistencyGuid atribuut on asustatud, Azure AD ühenduse siis ekspordib objekti Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2d142-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="2d142-p104">**Märkus:** Kui asutusesisese AD objekti imporditakse Azure AD ühenduse (st imporditud AD konnektori ruumi ja metaversumi viia), selle sourceAnchor väärtuseks ei saa enam muuta. Täpsustada sourceAnchor väärtus on esitatud asutusesisese AD objekti, konfigureerima oma vaevuste ConsistencyGuid atribuut see imporditakse Azure AD ühenduse.</span><span class="sxs-lookup"><span data-stu-id="2d142-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="2d142-111">SourceAnchor ja ConsistencyGuid kohta lisateabe saamiseks vaadake järgmist: [Azure AD ühenduse: kujundada mõisted](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="2d142-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

