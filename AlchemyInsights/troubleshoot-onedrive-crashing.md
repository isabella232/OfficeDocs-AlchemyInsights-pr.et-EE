---
title: OneDrive'i krahhide tõrkeotsing
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826195"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="093db-102">OneDrive'i krahhide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="093db-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="093db-103">Kui OneDrive jookseb korduvalt kokku, proovige järgmisi tõrkeotsingutoiminguid.</span><span class="sxs-lookup"><span data-stu-id="093db-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="093db-104">**Veenduge, et registrivõtmed poleks määratud.**</span><span class="sxs-lookup"><span data-stu-id="093db-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="093db-105">Liikuge registriredaktori abil HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="093db-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="093db-106">Kui DisableFileSyncNGSC on olemas ja selle väärtuseks on seatud 1, avage klahv ja muutke väärtus väärtuseks 0.</span><span class="sxs-lookup"><span data-stu-id="093db-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="093db-107">OneDrive'i käsitsi käivitamiseks valige Start</span><span class="sxs-lookup"><span data-stu-id="093db-107">Manually launch OneDrive by going to Start</span></span> ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="093db-109">, tippige otsinguväljale OneDrive ja seejärel klõpsake OneDrive'i töölauarakendust.</span><span class="sxs-lookup"><span data-stu-id="093db-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="093db-110">**OneDrive'i lähtestamine.**</span><span class="sxs-lookup"><span data-stu-id="093db-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="093db-111">Märkmed:</span><span class="sxs-lookup"><span data-stu-id="093db-111">Notes:</span></span>

- <span data-ttu-id="093db-112">OneDrive'i lähtestamisel katkestatakse kõik olemasolevad sünkroonimisühendused (sh teie isiklik OneDrive, kui see on häälestatud).</span><span class="sxs-lookup"><span data-stu-id="093db-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="093db-113">Te ei kaota faile ega andmeid, kui lähtestate OneDrive'i oma arvutis.</span><span class="sxs-lookup"><span data-stu-id="093db-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="093db-114">**OneDrive'i lähtestamiseks tehke ühte järgmistest.**</span><span class="sxs-lookup"><span data-stu-id="093db-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="093db-115">Dialoogiboksi Käivita avamiseks vajutage klahvikombinatsiooni Windowsi klahv ja R.</span><span class="sxs-lookup"><span data-stu-id="093db-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="093db-116">Tippige %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja vajutage nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="093db-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="093db-117">Käsuaken võidakse kuvada lühidalt.</span><span class="sxs-lookup"><span data-stu-id="093db-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="093db-118">OneDrive'i käsitsi käivitamiseks valige Start</span><span class="sxs-lookup"><span data-stu-id="093db-118">Manually launch OneDrive by going to Start</span></span> ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="093db-120">, tippige otsinguväljale OneDrive ja seejärel klõpsake OneDrive'i töölauarakendust.</span><span class="sxs-lookup"><span data-stu-id="093db-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="093db-121">Märkmed:</span><span class="sxs-lookup"><span data-stu-id="093db-121">Notes:</span></span>

- <span data-ttu-id="093db-122">Kui otsustasite enne lähtestamist sünkroonida ainult mõned kaustad, peate seda uuesti tegema, kui sünkroonimine on lõpule viidud.</span><span class="sxs-lookup"><span data-stu-id="093db-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="093db-123">Lisateavet [leiate teemast Valige, milliseid OneDrive'i kaustu arvutiga](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   sünkroonida.</span><span class="sxs-lookup"><span data-stu-id="093db-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="093db-124">Peate selle lõpule viima isikliku OneDrive'i ja OneDrive for Businessi jaoks.</span><span class="sxs-lookup"><span data-stu-id="093db-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>