---
title: SharePoint Online ahendamine
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761255"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="28293-102">SharePoint Online ahendamine</span><span class="sxs-lookup"><span data-stu-id="28293-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="28293-103">Kasutajad võivad saada 503 server on hõivatud tõrge, kui proovite liikuda OneDrive'i või SharePointi saidid.</span><span class="sxs-lookup"><span data-stu-id="28293-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="28293-104">See tõrge võib olla põhjustatud ahendamise teenuses SharePoint.</span><span class="sxs-lookup"><span data-stu-id="28293-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="28293-105">SharePoint Online kasutab ahendamise säilitada optimaalse jõudluse ja usaldusväärsuse teenuse SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="28293-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="28293-106">Vähendanud piiranguid arvu kasutajate toiminguid või samaaegsete kutsub (skript või kood) ressursside liigse kasutamise vältimiseks.</span><span class="sxs-lookup"><span data-stu-id="28293-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="28293-107">Kui te saada pärsitud, 99% ajast on kohandatud koodi tõttu.</span><span class="sxs-lookup"><span data-stu-id="28293-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="28293-108">Rohkem infot ahendamise vt [vältida pärsitud või SharePoint Online'i blokeeritud](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="28293-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="28293-109">Kui arvate, et see viga ei ole seotud ahendamise, kontrollige kas aktiivne hooldus toimub teie rentniku [sõnumikeskuse](https://portal.office.com/adminportal/home#/MessageCenter)kaudu.</span><span class="sxs-lookup"><span data-stu-id="28293-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="28293-110">Lõpuks tagama kontrollimiseks mis tahes teateid/intsidente, mis võib aset [Teenuseid tervise](https://portal.office.com/adminportal/home#/servicehealth) lehte külastades.</span><span class="sxs-lookup"><span data-stu-id="28293-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

