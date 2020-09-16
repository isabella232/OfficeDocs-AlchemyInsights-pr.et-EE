---
title: ConsistencyGuid/sourceAnchor käitumine
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756279"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="6efb8-102">ConsistencyGuid/sourceAnchor käitumine</span><span class="sxs-lookup"><span data-stu-id="6efb8-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="6efb8-103">Azure AD Connect (versioon 1.1.524.0 ja After) hõlbustab nüüd luu-ja lihaskonna vaevuste-ConsistencyGuid kasutamist kui sourceAnchor atribuuti.</span><span class="sxs-lookup"><span data-stu-id="6efb8-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="6efb8-104">Selle funktsiooni kasutamisel konfigureerib Azure AD Connect automaatselt sünkroonimise reeglid.</span><span class="sxs-lookup"><span data-stu-id="6efb8-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="6efb8-105">Kasutage luu-ja lihaskonna vaevusi – ConsistencyGuid sourceAnchor atribuuti.</span><span class="sxs-lookup"><span data-stu-id="6efb8-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="6efb8-106">ObjectGUID kasutatakse muud tüüpi objektide puhul.</span><span class="sxs-lookup"><span data-stu-id="6efb8-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="6efb8-107">Kui kohapealne AD kasutaja objekt, mille luu-ja lihaskonna vaevuse-ConsistencyGuid atribuut pole asustatud, kirjutab Azure AD Connect selle objectGUID väärtuseks tagasi kohapealses Active Directorys asuvasse luu-ja lihaskonna vaevuste-ConsistencyGuid atribuuti.</span><span class="sxs-lookup"><span data-stu-id="6efb8-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="6efb8-108">Pärast seda, kui luu-ja lihaskonna vaevusi-ConsistencyGuid atribuut on asustatud, eksporditakse Azure AD ja seejärel eksporditakse objekt Azure AD</span><span class="sxs-lookup"><span data-stu-id="6efb8-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="6efb8-109">**Märkus:** Kui kohapealne AD objekt imporditakse Azure AD Connect (see tähendab, et see on imporditud AD Connectori ruumi ja kavandatakse metaversumi), ei saa te selle sourceAnchor enam muuta.</span><span class="sxs-lookup"><span data-stu-id="6efb8-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="6efb8-110">Antud kohapealse reklaami objekti sourceAnchor määramiseks Konfigureerige selle luu-ja lihaskonna vaevuste-ConsistencyGuid atribuut, enne kui see imporditakse Azure AD Connecti.</span><span class="sxs-lookup"><span data-stu-id="6efb8-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="6efb8-111">Lisateavet SourceAnchor ja ConsistencyGuid kohta leiate järgmistest teemadest: [AZURE ad Connect: kujunduse kontseptsioonid](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="6efb8-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

