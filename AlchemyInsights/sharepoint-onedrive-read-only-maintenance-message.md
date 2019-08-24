---
title: Hooldus sõnumi kui üritatakse kasutada OneDrive'i või SharePointi kirjutuskaitstud
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620719"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="7fbe7-102">Hooldus sõnumi kui üritatakse kasutada OneDrive'i või SharePointi kirjutuskaitstud</span><span class="sxs-lookup"><span data-stu-id="7fbe7-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="7fbe7-103">Kasutajatele võidakse kuvada teade, **Registripidamise kirjutuskaitstud** , kui üritatakse kasutada OneDrive'i või SharePointi ühel järgmistest juhtudest.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="7fbe7-104">Plaanitud või aktiivne hooldus tegevus.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="7fbe7-105">Neid [Sõnumikeskuse](https://portal.office.com/adminportal/home#/messagecenter)kaudu otsima.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="7fbe7-106">Eelisõigus, tegevteenistuses vahejuhtumist, mis oleks toimunud.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="7fbe7-107">Teated/juhtumite kaudu [Teenuseid tervise](https://portal.office.com/adminportal/home#/servicehealth)kontrolli.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="7fbe7-108">Kerge automaatne probleemilahendus taastamise stsenaarium, mis võib juhtuda ootamatuid olukordi tõttu servereid, mis võib kesta vähem kui 30 min või nii.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="7fbe7-109">Ei ole keskus või teenuseid tervise konteerib nende väikeste kirjendamiseks, kuid tuleb peagi tagasi normaalseks.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="7fbe7-110">Väga vähestel juhtudel jälgisime ühel eespool loetletud kolme juhtudest on põhjuseks ja teenus on taastatud, et kasutajad brauseri vahemälu ei ole kummutatud.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="7fbe7-111">Proovige enne saidil navigeerimise brauseri vahemälu tühjendamine.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="7fbe7-112">Microsoft Edge brauseris, valige **seaded**ja valige **privaatsuse ja turvalisuse**.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="7fbe7-113">Valige jaotises **selge sirvimiseks** **Valige kustutatav**.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="7fbe7-114">Valige **küpsised ja salvestatud veebisaidiandmed**ja valige **selge**.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="7fbe7-115">Järgmiselt võib erineda kasutades teisi brauserid, nagu Mozilla Firefox või Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="7fbe7-116">Teine võimalus oleks avada SharePointi saidile või OneDrive Uus InPrivate-aken.</span><span class="sxs-lookup"><span data-stu-id="7fbe7-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>