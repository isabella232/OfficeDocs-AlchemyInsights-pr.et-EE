---
title: Kirjutuskaitstud, kui proovite kasutada SharePointi või OneDrive ' i
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670828"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="f8c72-102">Kirjutuskaitstud, kui proovite kasutada SharePointi või OneDrive ' i</span><span class="sxs-lookup"><span data-stu-id="f8c72-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="f8c72-103">Kui proovite SharePointi või OneDrive ' i kasutada mõnda järgmistest olukordadest, võivad kasutajad **lugeda** kirjutuskaitstud.</span><span class="sxs-lookup"><span data-stu-id="f8c72-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="f8c72-104">Plaanitud või aktiivne hooldustööd.</span><span class="sxs-lookup"><span data-stu-id="f8c72-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="f8c72-105">Nende otsimiseks liikuge [sõnumikeskuse](https://portal.office.com/adminportal/home#/messagecenter)kaudu.</span><span class="sxs-lookup"><span data-stu-id="f8c72-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="f8c72-106">Kõrge prioriteediga aktiivne teenuse juhtum, mis võib toimuda.</span><span class="sxs-lookup"><span data-stu-id="f8c72-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="f8c72-107">Saate otsida mis tahes nõuandjaid/intsidente, kui navigeerite [teenuse tervist](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f8c72-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="f8c72-108">Väike automaatse tervendamise stsenaarium, mis võib toimuda ootamatute sündmuste tõttu serverites, mis võivad kesta vähem kui 30 min või nii.</span><span class="sxs-lookup"><span data-stu-id="f8c72-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="f8c72-109">Neid väiksemaid tagasinõudmised pole sõnumikeskuse või teenuse tervislikke ametikohti, kuid sa peaksid olema väga kiiresti tagasi normaalne.</span><span class="sxs-lookup"><span data-stu-id="f8c72-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="f8c72-110">Väga vähestel juhtudel oleme täheldanud, et mõni eespool loetletud kolmest stsenaariumist on põhjus ja teenus on taastatud, kuid kasutajate brauseri vahemälu pole lahendatud.</span><span class="sxs-lookup"><span data-stu-id="f8c72-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="f8c72-111">Enne saidile navigeerimist proovige brauseri vahemälu tühjendada.</span><span class="sxs-lookup"><span data-stu-id="f8c72-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="f8c72-112">Valige Microsoft Edge ' i brauseris **sätted**ja seejärel valige **Privaatsus ja turve**.</span><span class="sxs-lookup"><span data-stu-id="f8c72-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="f8c72-113">Valige jaotises **Tühjenda sirvimine**käsk **Vali, mida soovite kustutada**.</span><span class="sxs-lookup"><span data-stu-id="f8c72-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="f8c72-114">Valige **küpsised ja salvestatud veebisaitide andmed**ning valige **Kustuta**.</span><span class="sxs-lookup"><span data-stu-id="f8c72-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="f8c72-115">Need toimingud võivad muude brauserite (nt Mozilla Firefoxi või Google Chrome ' i) kasutamisel erineda.</span><span class="sxs-lookup"><span data-stu-id="f8c72-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="f8c72-116">Teine võimalus on avada SharePointi sait või OneDrive uues InPrivate-aknas.</span><span class="sxs-lookup"><span data-stu-id="f8c72-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>