---
title: Kohandatud teatiste saatmine Intune ' iga
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992309"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="7d7ee-102">Kuidas saata kohandatud teated hallatud iOS-i ja Androidi seadmete kasutajatele</span><span class="sxs-lookup"><span data-stu-id="7d7ee-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="7d7ee-103">Intune ' i kohandatud teatisi töötleb ettevõtte portaali rakendus kasutaja seadmes.</span><span class="sxs-lookup"><span data-stu-id="7d7ee-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="7d7ee-104">Rakendus loob seejärel push teate selle seadme.</span><span class="sxs-lookup"><span data-stu-id="7d7ee-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="7d7ee-105">Järgmised on seadme eeltingimused kohandatud teatiste vastuvõtmise toetamiseks ja rakenduse loomiseks tõukemärguannet:</span><span class="sxs-lookup"><span data-stu-id="7d7ee-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="7d7ee-106">Seadmel peab olema installitud ettevõtteportaali rakendus.</span><span class="sxs-lookup"><span data-stu-id="7d7ee-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="7d7ee-107">Seade peab lubama ettevõtte portaali rakendusel tõukemärguandeid saata.</span><span class="sxs-lookup"><span data-stu-id="7d7ee-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="7d7ee-108">Kui rakendus on installitud või värskendatud, küsib kasutaja luba märguandeid.</span><span class="sxs-lookup"><span data-stu-id="7d7ee-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="7d7ee-109">Androidi seadmetel peab olema installitud Google Play teenused.</span><span class="sxs-lookup"><span data-stu-id="7d7ee-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="7d7ee-110">Seade tuleb registreerida Intune ' iga.</span><span class="sxs-lookup"><span data-stu-id="7d7ee-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="7d7ee-111">Lisateavet selle kohta, kuidas sõnumit saata, leiate [funktsiooni dokumentatsioonist](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="7d7ee-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
