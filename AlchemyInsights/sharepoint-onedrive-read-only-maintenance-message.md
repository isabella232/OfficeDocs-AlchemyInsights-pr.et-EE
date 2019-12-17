---
title: Kirjutuskaitstud hoolduse sõnumi katsel kasutada SharePointi või OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051277"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="b9930-102">Kirjutuskaitstud hoolduse sõnumi katsel kasutada SharePointi või OneDrive</span><span class="sxs-lookup"><span data-stu-id="b9930-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="b9930-103">Kasutajad võivad saada **kirjutuskaitstud hoolduse** sõnumi katsel kasutada SharePointi või OneDrive üks järgmistest tingimustest.</span><span class="sxs-lookup"><span data-stu-id="b9930-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="b9930-104">Planeeritud või aktiivne hooldustegevus.</span><span class="sxs-lookup"><span data-stu-id="b9930-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="b9930-105">Kontrollige neid, liikudes [sõnumikeskuse](https://portal.office.com/adminportal/home#/messagecenter)juurde.</span><span class="sxs-lookup"><span data-stu-id="b9930-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="b9930-106">Kõrge prioriteediga aktiivne teenindusjuhtum, mis võib tekkida.</span><span class="sxs-lookup"><span data-stu-id="b9930-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="b9930-107">Kontrollige kõik nõud/intsidendid navigeerides [teenuse tervis](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b9930-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="b9930-108">Väike auto-tervendav taastamise stsenaarium, mis võib juhtuda ootamatu sündmuste serverid, mis võivad kesta vähem kui 30 min või nii.</span><span class="sxs-lookup"><span data-stu-id="b9930-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="b9930-109">Nende väiksemate tagasimaksete jaoks pole sõnumikeskust ega teenuse Health postitusi, kuid peaksite varsti tagasi normaalseks.</span><span class="sxs-lookup"><span data-stu-id="b9930-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="b9930-110">Väga vähe kordi me täheldas, et üks eespool loetletud kolmest stsenaariumit on põhjus ja teenus on taastatud, kuid kasutajate brauseri vahemälu ei ole lahendatud.</span><span class="sxs-lookup"><span data-stu-id="b9930-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="b9930-111">Palun proovige tühjendada brauseri vahemälu enne navigeerimist saidile.</span><span class="sxs-lookup"><span data-stu-id="b9930-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="b9930-112">Valige oma Microsoft Edge ' i brauseris **sätted**ja seejärel **Privaatsus ja turve**.</span><span class="sxs-lookup"><span data-stu-id="b9930-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="b9930-113">Valige jaotises **Tühjenda sirvimine**käsk **Vali, mida tühjendada**.</span><span class="sxs-lookup"><span data-stu-id="b9930-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="b9930-114">Valige **küpsised ja salvestatud veebisaidi andmed**ning valige **Tühjenda**.</span><span class="sxs-lookup"><span data-stu-id="b9930-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="b9930-115">Need sammud võivad erineda, kui kasutate muid brausereid nagu Mozilla Firefox või Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="b9930-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="b9930-116">Teine võimalus oleks avada SharePointi saidi või OneDrive uues InPrivate-aknas.</span><span class="sxs-lookup"><span data-stu-id="b9930-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>