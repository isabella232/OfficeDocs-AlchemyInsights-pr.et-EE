---
title: E-posti profiilide kasutamine Intune ' i abil
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554978"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="355f9-102">E-posti profiilide kasutamine Intune ' i abil</span><span class="sxs-lookup"><span data-stu-id="355f9-102">Using email profiles with Intune</span></span>

<span data-ttu-id="355f9-103">Intune ' i abil saab luua ja juurutada mitmekeelseid meilikontosid (sisseehitatud) meiliklient mitme seadme platvormidel.</span><span class="sxs-lookup"><span data-stu-id="355f9-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="355f9-104">Lisateavet e-posti profiilidega seotud piirangute kohta (sh olemasolevate profiilide olemasolu ja selle kohta, kuidas eemaldada e-posti profiilid) leiate teemast [meilikontode lisamine seadmetele, mis kasutavad Intune](https://docs.microsoft.com/intune/email-settings-configure)' i.</span><span class="sxs-lookup"><span data-stu-id="355f9-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="355f9-105">Lisateavet iga seadme platvormi jaoks meiliprofiili loomise kohta leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="355f9-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="355f9-106">Androidi seadme sätted meili, autentimise ja sünkroonimise häälestamiseks Intune ' is</span><span class="sxs-lookup"><span data-stu-id="355f9-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="355f9-107">IOS-i ja iPadOS seadmete meilikontode lisamine Microsoft Intune ' is</span><span class="sxs-lookup"><span data-stu-id="355f9-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="355f9-108">Microsoft Intune ' i meilikonto sätted Windows Phone ' i 8,1 seadmete jaoks</span><span class="sxs-lookup"><span data-stu-id="355f9-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="355f9-109">Microsoft Intune ' is Windows 10 kasutavatele seadmetele mõeldud meilikontode meilisätted</span><span class="sxs-lookup"><span data-stu-id="355f9-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="355f9-110">**Levinud sünkroonimise probleem**</span><span class="sxs-lookup"><span data-stu-id="355f9-110">**Common syncing issue**</span></span>

<span data-ttu-id="355f9-111">**Rakenduse KNOX Androidi meilikontos takistab kasutajate kontakte, kalendrit ja tööülesandeid, mida sünkroonitakse kasutaja seadmetega.**</span><span class="sxs-lookup"><span data-stu-id="355f9-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="355f9-112">KNOX Android KNOXi meilikonto profiilis annab administraatorile võimaluse otsustada, milliseid sisutüüpe sünkroonitakse seadmesse, seades need lubatud.</span><span class="sxs-lookup"><span data-stu-id="355f9-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="355f9-113">Kui mis tahes sisutüübi säte on seatud **pole konfigureeritud** (vaikesäte), ei sünkroonita seda sisutüüpi automaatselt.</span><span class="sxs-lookup"><span data-stu-id="355f9-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="355f9-114">Kasutaja võib lubada sisutüübi, mida nad soovivad otse seadmele käsitsi lisada, kuid see konfiguratsioon kirjutatakse üle Intune ' i Poliitikasätte ja selle sisutüübi sünkroonimine peatub.</span><span class="sxs-lookup"><span data-stu-id="355f9-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

