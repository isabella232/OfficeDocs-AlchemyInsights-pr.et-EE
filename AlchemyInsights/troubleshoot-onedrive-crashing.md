---
title: OneDrive'i krahhide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748917"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="24ff8-102">OneDrive'i krahhide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="24ff8-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="24ff8-103">Kui OneDrive jookseb korduvalt kokku, proovige järgmisi veaotsingu toiminguid.</span><span class="sxs-lookup"><span data-stu-id="24ff8-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="24ff8-104">**Veenduge, et registrivõtmeid pole seatud:**</span><span class="sxs-lookup"><span data-stu-id="24ff8-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="24ff8-105">Registriredaktori abil liikuge HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="24ff8-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="24ff8-106">Kui DisableFileSyncNGSC on olemas ja seatud 1, avage võti ja muutke väärtuseks 0.</span><span class="sxs-lookup"><span data-stu-id="24ff8-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="24ff8-107">OneDrive'i käsitsi käivitamiseks avage menüü Start</span><span class="sxs-lookup"><span data-stu-id="24ff8-107">Manually launch OneDrive by going to Start</span></span> ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="24ff8-109">, tippige otsinguväljale OneDrive ja seejärel klõpsake OneDrive'i töölauarakendust.</span><span class="sxs-lookup"><span data-stu-id="24ff8-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="24ff8-110">**OneDrive'i lähtestamine:**</span><span class="sxs-lookup"><span data-stu-id="24ff8-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="24ff8-111">Märkmed:</span><span class="sxs-lookup"><span data-stu-id="24ff8-111">Notes:</span></span>

- <span data-ttu-id="24ff8-112">OneDrive'i lähtestamine katkestab kõik olemasolevad sünkroonimisühendused (sh teie isikliku OneDrive'i, kui see on häälestatud).</span><span class="sxs-lookup"><span data-stu-id="24ff8-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="24ff8-113">OneDrive'i arvutist lähtestamisel faile ega andmeid ei kaotata.</span><span class="sxs-lookup"><span data-stu-id="24ff8-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="24ff8-114">**OneDrive'i lähtestamiseks**</span><span class="sxs-lookup"><span data-stu-id="24ff8-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="24ff8-115">Avab dialoogi Käivita, vajutades Windowsi klahvi ja r.</span><span class="sxs-lookup"><span data-stu-id="24ff8-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="24ff8-116">Tippige %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja vajutage nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="24ff8-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="24ff8-117">Käsuaken võidakse kuvada korraks.</span><span class="sxs-lookup"><span data-stu-id="24ff8-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="24ff8-118">OneDrive'i käsitsi käivitamiseks avage menüü Start</span><span class="sxs-lookup"><span data-stu-id="24ff8-118">Manually launch OneDrive by going to Start</span></span> ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="24ff8-120">, tippige otsinguväljale OneDrive ja seejärel klõpsake OneDrive'i töölauarakendust.</span><span class="sxs-lookup"><span data-stu-id="24ff8-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="24ff8-121">Märkmed:</span><span class="sxs-lookup"><span data-stu-id="24ff8-121">Notes:</span></span>

- <span data-ttu-id="24ff8-122">Kui olete enne lähtestamist otsustanud sünkroonida ainult mõned kaustad, peate seda uuesti tegema, kui sünkroonimine on lõpule viidud.</span><span class="sxs-lookup"><span data-stu-id="24ff8-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="24ff8-123">Lisateabe [saamiseks lugege lisateavet jaotisest Valige, millised OneDrive'i kaustad arvutiga sünkroonida.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  </span><span class="sxs-lookup"><span data-stu-id="24ff8-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="24ff8-124">Peate selle oma isikliku OneDrive'i ja OneDrive for Businessi jaoks lõpule viima.</span><span class="sxs-lookup"><span data-stu-id="24ff8-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>