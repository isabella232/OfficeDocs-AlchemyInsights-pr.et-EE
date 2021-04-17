---
title: ConsistencyGuid / sourceAnchor behavior
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816988"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="8273f-102">ConsistencyGuid / sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="8273f-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="8273f-103">Azure AD Connect (versioon 1.1.524.0 ja pärast seda) hõlbustab nüüd msDS-ConsistencyGuidi kasutamist atribuudi sourceAnchorna.</span><span class="sxs-lookup"><span data-stu-id="8273f-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="8273f-104">Selle funktsiooni kasutamisel konfigureerib Azure AD Connect sünkroonimisreeglid automaatselt:</span><span class="sxs-lookup"><span data-stu-id="8273f-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="8273f-105">Kasutage atribuuti msDS-ConsistencyGuid user-objektide atribuudina sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="8273f-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="8273f-106">ObjectGUID-d kasutatakse muude objektitüüpide jaoks.</span><span class="sxs-lookup"><span data-stu-id="8273f-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="8273f-107">Mis tahes asutusesisese AD-kasutaja objekti puhul, mille atribuut msDS-ConsistencyGuid pole asustatud, kirjutab Azure AD Connect oma objektiGUID-väärtuse tagasi asutusesisese Active Directory atribuudile msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="8273f-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="8273f-108">Kui atribuut msDS-ConsistencyGuid on asustatud, ekspordib Azure AD Connect objekti Azure AD-sse.</span><span class="sxs-lookup"><span data-stu-id="8273f-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="8273f-109">**Märkus.** Kui kohapealne AD-objekt on azure AD Connecti imporditud (st imporditud AD Connectori ruumi ja prognoositud metaversumisse), ei saa te selle sourceAnchori väärtust enam muuta.</span><span class="sxs-lookup"><span data-stu-id="8273f-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="8273f-110">Antud asutusesisese AD-objekti atribuudi sourceAnchor määramiseks konfigureerige selle atribuut msDS-ConsistencyGuid enne selle importimist Azure AD Connecti.</span><span class="sxs-lookup"><span data-stu-id="8273f-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="8273f-111">Lisateavet SourceAnchori ja ConsistencyGuid kohta leiate järgmistest artiklitest: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="8273f-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

