---
title: ConsistencyGuid/sourceAnchor käitumine
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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516973"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="13e8d-102">ConsistencyGuid/sourceAnchor käitumine</span><span class="sxs-lookup"><span data-stu-id="13e8d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="13e8d-103">Azure AD ühenduse (versioon 1.1.524.0 ja pärast) nüüd hõlbustab msDS-ConsistencyGuid kasutamine sourceAnchor atribuut.</span><span class="sxs-lookup"><span data-stu-id="13e8d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="13e8d-104">Selle funktsiooni kasutamisel konfigureerib Azure AD Connect automaatselt sünkroonimisreeglid:</span><span class="sxs-lookup"><span data-stu-id="13e8d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="13e8d-105">Kasutage msDS-ConsistencyGuid kui sourceAnchor atribuut kasutaja objektid.</span><span class="sxs-lookup"><span data-stu-id="13e8d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="13e8d-106">ObjectGUID-i kasutatakse muude objektitüüpide puhul.</span><span class="sxs-lookup"><span data-stu-id="13e8d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="13e8d-107">Iga asutusesisese AD kasutaja objekti, mille msDS-ConsistencyGuid atribuut ei ole asustatud, Azure AD ühenduse kirjutab oma objectGUID väärtus tagasi on asutusesisese Active Directory atribuudi msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="13e8d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="13e8d-108">Pärast msDS-ConsistencyGuid atribuut on asustatud Azure AD ühenduse seejärel eksportida objekti Azure AD.</span><span class="sxs-lookup"><span data-stu-id="13e8d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="13e8d-109">**Märkus:** Kui asutusesisese AD objekti imporditakse Azure AD ühenduse (st imporditud AD connector Space ja prognoositud Metaverse), ei saa muuta selle sourceAnchor väärtus enam.</span><span class="sxs-lookup"><span data-stu-id="13e8d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="13e8d-110">Konkreetse asutusesisese AD objekti sourceAnchor väärtuse määramiseks Konfigureerige selle msDS-ConsistencyGuid atribuut enne importimist Azure AD ühenduse.</span><span class="sxs-lookup"><span data-stu-id="13e8d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="13e8d-111">SourceAnchor ja ConsistencyGuid kohta lisateabe saamiseks vaadake järgmist: [AZURE AD ühenduse: kujunduse mõisted](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="13e8d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

