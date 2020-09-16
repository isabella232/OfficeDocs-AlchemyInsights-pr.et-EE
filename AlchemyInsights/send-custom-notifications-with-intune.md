---
title: Kohandatud teatiste saatmine Intune ' i abil
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720642"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="7ef1b-102">Kohandatud teatiste saatmine hallatud iOS-i ja Androidi seadmete kasutajatele</span><span class="sxs-lookup"><span data-stu-id="7ef1b-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="7ef1b-103">Intune ' i jaoks kohandatud teatisi töötleb kasutaja seadmes ettevõtte portaali rakendus.</span><span class="sxs-lookup"><span data-stu-id="7ef1b-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="7ef1b-104">Seejärel loob rakendus selle seadme push-teatise.</span><span class="sxs-lookup"><span data-stu-id="7ef1b-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="7ef1b-105">Järgnevalt on toodud seadme eeltingimused kohandatud teatiste vastuvõtmise toetamiseks ja rakenduse loomiseks seejärel push Notification.</span><span class="sxs-lookup"><span data-stu-id="7ef1b-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="7ef1b-106">Seadmes peab olema installitud ettevõtte portaali rakendus.</span><span class="sxs-lookup"><span data-stu-id="7ef1b-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="7ef1b-107">Seade peab lubama ettevõtte portaali rakendusel saata push Notifications.</span><span class="sxs-lookup"><span data-stu-id="7ef1b-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="7ef1b-108">Kui rakendus on installitud või värskendatud, palutakse kasutajal teatised lubada.</span><span class="sxs-lookup"><span data-stu-id="7ef1b-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="7ef1b-109">Androidi seadmetes peab olema installitud Google Play teenused.</span><span class="sxs-lookup"><span data-stu-id="7ef1b-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="7ef1b-110">Seade peab olema varustatud Intune ' iga.</span><span class="sxs-lookup"><span data-stu-id="7ef1b-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="7ef1b-111">Lisateavet selle kohta, kuidas sõnumit saata, leiate [funktsiooni dokumentatsioonist](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="7ef1b-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
