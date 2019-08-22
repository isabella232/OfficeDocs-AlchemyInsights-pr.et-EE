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
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559836"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="48f63-102">SharePoint Online ahendamine</span><span class="sxs-lookup"><span data-stu-id="48f63-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="48f63-103">Kasutajad võivad saada 503 server on hõivatud tõrge, kui proovite liikuda OneDrive'i või SharePointi saidid.</span><span class="sxs-lookup"><span data-stu-id="48f63-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="48f63-104">See tõrge võib olla põhjustatud ahendamise teenuses SharePoint.</span><span class="sxs-lookup"><span data-stu-id="48f63-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="48f63-105">SharePoint Online kasutab ahendamise säilitada optimaalse jõudluse ja usaldusväärsuse teenuse SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="48f63-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="48f63-106">Vähendanud piiranguid arvu kasutajate toiminguid või samaaegsete kutsub (skript või kood) ressursside liigse kasutamise vältimiseks.</span><span class="sxs-lookup"><span data-stu-id="48f63-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="48f63-107">Kui te saada pärsitud, 99% ajast on kohandatud koodi tõttu.</span><span class="sxs-lookup"><span data-stu-id="48f63-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="48f63-108">Rohkem infot ahendamise vt [vältida pärsitud või SharePoint Online'i blokeeritud](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="48f63-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="48f63-109">Kui arvate, et see viga ei ole seotud ahendamise, kontrollige kas aktiivne hooldus toimub teie rentniku [sõnumikeskuse](https://portal.office.com/adminportal/home#/MessageCenter)kaudu.</span><span class="sxs-lookup"><span data-stu-id="48f63-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="48f63-110">Lõpuks tagama kontrollimiseks mis tahes teateid/intsidente, mis võib aset [Teenuseid tervise](https://portal.office.com/adminportal/home#/servicehealth) lehte külastades.</span><span class="sxs-lookup"><span data-stu-id="48f63-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

