---
title: ConsistencyGuid / sourceAnchor käitumine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408104"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="50353-102">ConsistencyGuid / sourceAnchor käitumine</span><span class="sxs-lookup"><span data-stu-id="50353-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="50353-103">Azure AD ühenduse loomine (versioon 1.1.524.0 ja pärast) nüüd lihtsustab kasutamist msDS-ConsistencyGuid kui sourceAnchor atribuut.</span><span class="sxs-lookup"><span data-stu-id="50353-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="50353-104">Kui kasutate seda funktsiooni, Azure AD ühenduse konfigureerib automaatselt sünkroonimise reeglid:</span><span class="sxs-lookup"><span data-stu-id="50353-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="50353-105">Kasutada msDS-ConsistencyGuid sourceAnchor atribuut kasutaja objektid.</span><span class="sxs-lookup"><span data-stu-id="50353-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="50353-106">FederatedIdentity kasutatakse muud objekti tüüpi.</span><span class="sxs-lookup"><span data-stu-id="50353-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="50353-107">Ühegi esitatud asutusesisese AD kasutaja objekti kelle vaevuste ConsistencyGuid atribuut ei sisestata, Azure AD ühenduse kirjutab oma FederatedIdentity väärtusena vaevuste ConsistencyGuid atribuut asutusesisese Active Directory.</span><span class="sxs-lookup"><span data-stu-id="50353-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="50353-108">Pärast vaevuste ConsistencyGuid atribuut on asustatud, Azure AD ühenduse siis ekspordib objekti Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50353-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="50353-109">**Märkus:** Kui asutusesisese AD objekti imporditakse Azure AD ühenduse (st imporditud AD konnektori ruumi ja metaversumi viia), selle sourceAnchor väärtuseks ei saa enam muuta.</span><span class="sxs-lookup"><span data-stu-id="50353-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="50353-110">Täpsustada sourceAnchor väärtus on esitatud asutusesisese AD objekti, konfigureerima oma vaevuste ConsistencyGuid atribuut see imporditakse Azure AD ühenduse.</span><span class="sxs-lookup"><span data-stu-id="50353-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="50353-111">SourceAnchor ja ConsistencyGuid kohta lisateabe saamiseks vaadake järgmist: [Azure AD ühenduse: kujundada mõisted](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="50353-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

