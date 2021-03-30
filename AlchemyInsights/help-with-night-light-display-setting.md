---
title: Öövalguse kuvamissätte spikker
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404399"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="9cab5-102">Öövalguse kuvamissätte spikker</span><span class="sxs-lookup"><span data-stu-id="9cab5-102">Help with the night light display setting</span></span>

<span data-ttu-id="9cab5-103">Ööaja kuvamissätete kohta leiate lisateavet teemast Windows 10 ööaja [kuvamisaja konfigureerimine.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="9cab5-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="9cab5-104">Kui öövalguse suvandid on jaotises Sätted tuhm, kontrollige oma kuvadraiverit.</span><span class="sxs-lookup"><span data-stu-id="9cab5-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="9cab5-105">Klõpsake tegumiribal otsinguvälja ja tippige **seadmehaldur** ja seejärel **valige** otsingutulemitest Seadmehaldur.</span><span class="sxs-lookup"><span data-stu-id="9cab5-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="9cab5-106">Laiendage **valikut Kuvaadapterid.**</span><span class="sxs-lookup"><span data-stu-id="9cab5-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="9cab5-107">Kahjuks pole öövalguse funktsioon saadaval, kui teie seade kasutab DisplayLinki draiverit või põhikuvadraiverit.</span><span class="sxs-lookup"><span data-stu-id="9cab5-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="9cab5-108">Öövalguse funktsioon kasutab hiljutist graafikatehnoloogiat, nii et võib juhtuda, et peate kuvadraiverit värskendama.</span><span class="sxs-lookup"><span data-stu-id="9cab5-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="9cab5-109">Värskenduste otsimiseks valige Start  >  **Settings**  >  **Update & Security** Windows  >  **Update** Check  >  **for Updates**....</span><span class="sxs-lookup"><span data-stu-id="9cab5-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="9cab5-110">OR</span><span class="sxs-lookup"><span data-stu-id="9cab5-110">OR</span></span>

- <span data-ttu-id="9cab5-111">Uusimate kuvadraiverite käsitsi allalaadimiseks ja installimiseks külastage riistvara tootja tugiteenuste veebisaiti.</span><span class="sxs-lookup"><span data-stu-id="9cab5-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="9cab5-112">Öine tule lähtestamine registris</span><span class="sxs-lookup"><span data-stu-id="9cab5-112">Reset night light in the registry</span></span>

<span data-ttu-id="9cab5-113">Kui kuvadraiveri värskendamine ei toiminud, peate võib-olla lähtestama registris öövalguse.</span><span class="sxs-lookup"><span data-stu-id="9cab5-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="9cab5-114">**Ettevaatust.** See tõrkeotsingut juhis on soovitatav ainult kogenud kasutajatele.</span><span class="sxs-lookup"><span data-stu-id="9cab5-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="9cab5-115">Kui muudate registrit valesti, võivad ilmneda tõsised probleemid.</span><span class="sxs-lookup"><span data-stu-id="9cab5-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="9cab5-116">Lisakaitse tagamiseks varundage register enne selle muutmist, et saate selle probleemide korral taastada.</span><span class="sxs-lookup"><span data-stu-id="9cab5-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="9cab5-117">Tippige otsinguväljale tekst **regedit** ja seejärel **valige** otsingutulemitest Registriredaktor.</span><span class="sxs-lookup"><span data-stu-id="9cab5-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="9cab5-118">Avage järgmine registrivõti.</span><span class="sxs-lookup"><span data-stu-id="9cab5-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="9cab5-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="9cab5-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="9cab5-120">Eksportige ja kustutage järgmine alamvõti:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="9cab5-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="9cab5-121">Eksportige ja kustutage järgmine alamvõti:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="9cab5-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="9cab5-122">Taaskäivitage Windows ja kontrollige, kas öövalgustuse suvandid on saadaval.</span><span class="sxs-lookup"><span data-stu-id="9cab5-122">Restart Windows and verify if the night light options are available.</span></span>


