---
title: ConsistencyGuid/sourceAnchor käitumine
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705729"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3dd91-102">ConsistencyGuid/sourceAnchor käitumine</span><span class="sxs-lookup"><span data-stu-id="3dd91-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3dd91-103">Azure AD ühenduse (versioon 1.1.524.0 ja pärast) nüüd hõlbustab msDS-ConsistencyGuid kasutamine sourceAnchor atribuut.</span><span class="sxs-lookup"><span data-stu-id="3dd91-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="3dd91-104">Selle funktsiooni kasutamisel konfigureerib Azure AD Connect automaatselt sünkroonimisreeglid:</span><span class="sxs-lookup"><span data-stu-id="3dd91-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3dd91-105">Kasutage msDS-ConsistencyGuid kui sourceAnchor atribuut kasutaja objektid.</span><span class="sxs-lookup"><span data-stu-id="3dd91-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="3dd91-106">ObjectGUID-i kasutatakse muude objektitüüpide puhul.</span><span class="sxs-lookup"><span data-stu-id="3dd91-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3dd91-107">Iga asutusesisese AD kasutaja objekti, mille msDS-ConsistencyGuid atribuut ei ole asustatud, Azure AD ühenduse kirjutab oma objectGUID väärtus tagasi on asutusesisese Active Directory atribuudi msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="3dd91-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="3dd91-108">Pärast msDS-ConsistencyGuid atribuut on asustatud Azure AD ühenduse seejärel eksportida objekti Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3dd91-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3dd91-109">**Märkus:** Kui asutusesisese AD objekti imporditakse Azure AD ühenduse (st imporditud AD connector Space ja prognoositud Metaverse), ei saa muuta selle sourceAnchor väärtus enam.</span><span class="sxs-lookup"><span data-stu-id="3dd91-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="3dd91-110">Konkreetse asutusesisese AD objekti sourceAnchor väärtuse määramiseks Konfigureerige selle msDS-ConsistencyGuid atribuut enne importimist Azure AD ühenduse.</span><span class="sxs-lookup"><span data-stu-id="3dd91-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3dd91-111">SourceAnchor ja ConsistencyGuid kohta lisateabe saamiseks vaadake järgmist: [AZURE AD ühenduse: kujunduse mõisted](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3dd91-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

