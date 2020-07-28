---
title: Kaotsiläinud iOS-i seadmete leidmine Intune ' i abil
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439144"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="7ce06-102">Kaotsiläinud iOS-i seadmete leidmine Intune ' i abil</span><span class="sxs-lookup"><span data-stu-id="7ce06-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="7ce06-103">IOS-i seadmes kaotatud režiimi lubamine võimaldab administraatoril kuvada lukustuskuval sõnumi ja kontaktisiku telefoninumbri.</span><span class="sxs-lookup"><span data-stu-id="7ce06-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="7ce06-104">Pärast kaotatud režiimi lubamist saab administraator kasutada seadme asukoha tuvastamiseks seadme asukohta.</span><span class="sxs-lookup"><span data-stu-id="7ce06-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="7ce06-105">Seadme asukoha tuvastamine Intune ' is töötab koos iOS-i seadmetega, et kuvada kindla seadme asukoht kaardil.</span><span class="sxs-lookup"><span data-stu-id="7ce06-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="7ce06-106">Selle toimingu kasutamiseks peab iOS-i seade olema:</span><span class="sxs-lookup"><span data-stu-id="7ce06-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="7ce06-107">Juhendav režiim</span><span class="sxs-lookup"><span data-stu-id="7ce06-107">Supervised mode</span></span>
- <span data-ttu-id="7ce06-108">Kaotatud režiim</span><span class="sxs-lookup"><span data-stu-id="7ce06-108">Lost mode</span></span>

<span data-ttu-id="7ce06-109">Lisateavet leiate teemast [kaotsiläinud režiimi lubamine iOS-i/iPadOS seadmetes, kus](https://docs.microsoft.com/intune/device-lost-mode) on Intune ' is kaotatud [või varastatud iOS-i/iPadOS seadmete otsimine](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="7ce06-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="7ce06-110">**KKK**</span><span class="sxs-lookup"><span data-stu-id="7ce06-110">**FAQ**</span></span>

<span data-ttu-id="7ce06-111">K: ma väljastasin serveri toimingu, et eemaldada seadmest ettevõtte andmed ja nüüd on see ootel olekus kinni.</span><span class="sxs-lookup"><span data-stu-id="7ce06-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="7ce06-112">V: serveri toimingu edukaks lõpuleviimiseks peab sihipärane seade olema võrgus ja terve.</span><span class="sxs-lookup"><span data-stu-id="7ce06-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="7ce06-113">Järgmistes olukordades jääb kaugprotseduurikutse 30 päevaks ootel olekusse või ajani, mil seade selle käsu kinnitab.</span><span class="sxs-lookup"><span data-stu-id="7ce06-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="7ce06-114">Kui seadmel pole ühenduvust</span><span class="sxs-lookup"><span data-stu-id="7ce06-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="7ce06-115">Kui seade kaotab oma juhtimise oleku Intune ' iga</span><span class="sxs-lookup"><span data-stu-id="7ce06-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="7ce06-116">Kui arvate, et seade ei kontrolli enam ja et see ei saa ettevõtte andmeid eemaldada, valige Kustuta.</span><span class="sxs-lookup"><span data-stu-id="7ce06-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="7ce06-117">Kustutamine eemaldab seadme kirje nii, et seda ei kuvata enam seadmete loendis.</span><span class="sxs-lookup"><span data-stu-id="7ce06-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="7ce06-118">Kui seade muutub taas aktiivseks, peab selle kasutaja selle uuesti registreerima.</span><span class="sxs-lookup"><span data-stu-id="7ce06-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="7ce06-119">K: Miks pole teatud serveri toimingud minu jaoks saadaval?</span><span class="sxs-lookup"><span data-stu-id="7ce06-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="7ce06-120">V: kõik platvormid ei toeta kõiki serveri seadme toiminguid.</span><span class="sxs-lookup"><span data-stu-id="7ce06-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="7ce06-121">Järgmised serveri toimingud on platvormile omased, nii et need on saadaval ainult nende platvormide jaoks, mida on märgitud.</span><span class="sxs-lookup"><span data-stu-id="7ce06-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="7ce06-122">Ümbersõit Activation Lock (ainult iOS)</span><span class="sxs-lookup"><span data-stu-id="7ce06-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="7ce06-123">Värske algus (ainult Windows)</span><span class="sxs-lookup"><span data-stu-id="7ce06-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="7ce06-124">Lost Mode (ainult iOS)</span><span class="sxs-lookup"><span data-stu-id="7ce06-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="7ce06-125">Seadme leidmine (ainult iOS)</span><span class="sxs-lookup"><span data-stu-id="7ce06-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="7ce06-126">Taaskäivita (ainult Windows)</span><span class="sxs-lookup"><span data-stu-id="7ce06-126">Restart (Windows only)</span></span>

<span data-ttu-id="7ce06-127">Iga toimingu kohta leiate lisateavet teemast [Saadaolevad seadme toimingud](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="7ce06-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>