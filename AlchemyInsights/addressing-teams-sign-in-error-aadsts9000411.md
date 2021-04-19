---
title: Teamsi sisselogimistõrge AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821983"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="33f64-102">Teamsi sisselogimistõrge AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="33f64-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="33f64-103">Microsoft Teamsi sisselogimisel võidakse kuvada tõrketeade: Kahjuks on meil probleeme **AADSTS9000411i sisselogimisega: taotlus pole õigesti vormindatud. Parameeter "login_hint" on dubleeritud.**</span><span class="sxs-lookup"><span data-stu-id="33f64-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="33f64-104">Selle probleemi lahendamiseks veenduge, et teie Microsoft Teamsi kliente värskendatakse.</span><span class="sxs-lookup"><span data-stu-id="33f64-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="33f64-105">Lisateavet kliendi värskendamise kohta leiate teemast [Microsoft Teamsi värskendamine.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="33f64-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="33f64-106">Kui te ei saa mingil põhjusel klientrakendust värskendada, tühjendab klientrakendusest väljalogimine enamik vahemällu talletatud andmeid.</span><span class="sxs-lookup"><span data-stu-id="33f64-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="33f64-107">Kui teil on pärast sisselogimist endiselt probleeme, sulgege Teams ja tühjendage oma kliendi vahemälu, tehes järgmist.</span><span class="sxs-lookup"><span data-stu-id="33f64-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="33f64-108">Sulgege Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="33f64-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="33f64-109">Avage: %appdata%\microsoft\teams ja kustutage kõik failid.</span><span class="sxs-lookup"><span data-stu-id="33f64-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="33f64-110">Avage Microsoft Teams uuesti.</span><span class="sxs-lookup"><span data-stu-id="33f64-110">Reopen Microsoft Teams.</span></span>
