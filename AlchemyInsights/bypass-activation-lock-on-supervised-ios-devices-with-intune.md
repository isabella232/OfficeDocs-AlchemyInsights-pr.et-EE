---
title: Intune ' i aktiveerimise lukustus juhendatud iOS-i seadmetes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423730"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="c16b8-102">Intune ' i aktiveerimise lukustus juhendatud iOS-i seadmetes</span><span class="sxs-lookup"><span data-stu-id="c16b8-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="c16b8-103">IOS-i seadmetes aktiveerimise lukustusest loobumise võimalus hõlbustab stsenaariumist taastumist, kui kasutaja lubab aktiveerimise lukustuse ettevõtte seadmes ja seejärel lahkub ettevõttest.</span><span class="sxs-lookup"><span data-stu-id="c16b8-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="c16b8-104">Aktiveerimise lukustusest möödumiseks on eeltingimused järgmised.</span><span class="sxs-lookup"><span data-stu-id="c16b8-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="c16b8-105">Seade on "järelevalve all".</span><span class="sxs-lookup"><span data-stu-id="c16b8-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="c16b8-106">Aktiveerimise lukustus on edukalt lubatud, kasutades iOS-i seadme piiramise poliitikat Intune ' is.</span><span class="sxs-lookup"><span data-stu-id="c16b8-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="c16b8-107">Lisaks peaksite aktiveerimise lukustusest loobumisel tegema järgmist.</span><span class="sxs-lookup"><span data-stu-id="c16b8-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="c16b8-108">Seadme tühjendamine füüsiliselt.</span><span class="sxs-lookup"><span data-stu-id="c16b8-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="c16b8-109">Kopeerige kood enne pühi väljastamist.</span><span class="sxs-lookup"><span data-stu-id="c16b8-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="c16b8-110">**Märkus:** Pühkige kood ei ole tõstutundlik, seega pole märke "-" ei nõuta.</span><span class="sxs-lookup"><span data-stu-id="c16b8-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="c16b8-111">Lisateavet leiate teemast [aktiveerimise lukustuse tühistamine iOS-i seadmetes, kus on Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="c16b8-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="c16b8-112">**KKK**</span><span class="sxs-lookup"><span data-stu-id="c16b8-112">**FAQ**</span></span>

<span data-ttu-id="c16b8-113">K: **ma väljastasin serveri toimingu, et eemaldada seadmest ettevõtte andmed ja nüüd on see ootel olekus kinni.**</span><span class="sxs-lookup"><span data-stu-id="c16b8-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="c16b8-114">V: serveri toimingu edukaks lõpuleviimiseks peab sihipärane seade olema võrgus ja terve.</span><span class="sxs-lookup"><span data-stu-id="c16b8-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="c16b8-115">Järgmistes olukordades jääb kaugprotseduurikutse 30 päevaks ootel olekusse või ajani, kui seade on seadme kinnitanud.</span><span class="sxs-lookup"><span data-stu-id="c16b8-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="c16b8-116">Pole ühendust.</span><span class="sxs-lookup"><span data-stu-id="c16b8-116">Does not have connectivity.</span></span>
- <span data-ttu-id="c16b8-117">Kaotab oma juhtimise oleku Intune ' iga.</span><span class="sxs-lookup"><span data-stu-id="c16b8-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="c16b8-118">Kui arvate, et seade ei ole enam sisse möllitud ja et see ei eemalda ettevõtte andmeid, valige Kustuta.</span><span class="sxs-lookup"><span data-stu-id="c16b8-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="c16b8-119">Kustutamine eemaldab seadme kirje nii, et seda ei kuvata enam seadmete loendis.</span><span class="sxs-lookup"><span data-stu-id="c16b8-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="c16b8-120">Kui soovite, et seade saaks uuesti aktiivseks, peab selle kasutaja seadme uuesti registreerima.</span><span class="sxs-lookup"><span data-stu-id="c16b8-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="c16b8-121">K: **miks pole teatud serveri toimingud minu jaoks saadaval?**</span><span class="sxs-lookup"><span data-stu-id="c16b8-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="c16b8-122">V: kõik platvormid ei toeta kõiki serveri seadme toiminguid.</span><span class="sxs-lookup"><span data-stu-id="c16b8-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="c16b8-123">Järgmised Remote-toimingud on platvormile omased.</span><span class="sxs-lookup"><span data-stu-id="c16b8-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="c16b8-124">Ümbersõit Activation Lock (ainult iOS)</span><span class="sxs-lookup"><span data-stu-id="c16b8-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="c16b8-125">Värske algus (ainult Windows)</span><span class="sxs-lookup"><span data-stu-id="c16b8-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="c16b8-126">Lost Mode (ainult iOS)</span><span class="sxs-lookup"><span data-stu-id="c16b8-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="c16b8-127">Seadme leidmine (ainult iOS)</span><span class="sxs-lookup"><span data-stu-id="c16b8-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="c16b8-128">Taaskäivita (ainult Windows)</span><span class="sxs-lookup"><span data-stu-id="c16b8-128">Restart (Windows only)</span></span>

<span data-ttu-id="c16b8-129">Iga toimingu kohta leiate lisateavet teemast [Saadaolevad seadme toimingud](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="c16b8-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>