---
title: Kohandatud teatiste saatmine Intune ' iga
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886853"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="debf3-102">Kuidas saata kohandatud teated hallatud iOS-i ja Androidi seadmete kasutajatele</span><span class="sxs-lookup"><span data-stu-id="debf3-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="debf3-103">Intune ' i kohandatud teatisi töötleb ettevõtte portaali rakendus kasutaja seadmes.</span><span class="sxs-lookup"><span data-stu-id="debf3-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="debf3-104">Rakendus loob seejärel push teate selle seadme.</span><span class="sxs-lookup"><span data-stu-id="debf3-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="debf3-105">Järgmised on seadme eeltingimused kohandatud teatiste vastuvõtmise toetamiseks ja rakenduse loomiseks tõukemärguannet:</span><span class="sxs-lookup"><span data-stu-id="debf3-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="debf3-106">Seadmel peab olema installitud ettevõtteportaali rakendus.</span><span class="sxs-lookup"><span data-stu-id="debf3-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="debf3-107">Seade peab lubama ettevõtte portaali rakendusel tõukemärguandeid saata.</span><span class="sxs-lookup"><span data-stu-id="debf3-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="debf3-108">Kui rakendus on installitud või värskendatud, küsib kasutaja luba märguandeid.</span><span class="sxs-lookup"><span data-stu-id="debf3-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="debf3-109">Androidi seadmetel peab olema installitud Google Play teenused.</span><span class="sxs-lookup"><span data-stu-id="debf3-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="debf3-110">Seade tuleb registreerida Intune ' iga.</span><span class="sxs-lookup"><span data-stu-id="debf3-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="debf3-111">Lisateavet selle kohta, kuidas sõnumit saata, leiate [funktsiooni dokumentatsioonist](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="debf3-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
