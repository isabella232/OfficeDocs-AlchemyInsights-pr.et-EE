---
title: OneDrive ' i tõrkeotsing jookseb kokku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664994"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="34daf-102">OneDrive ' i tõrkeotsing jookseb kokku</span><span class="sxs-lookup"><span data-stu-id="34daf-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="34daf-103">Kui OneDrive jookseb korduvalt kokku, proovige järgmisi veaotsingu toiminguid.</span><span class="sxs-lookup"><span data-stu-id="34daf-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="34daf-104">**Veenduge, et registrivõtmed pole määratud.**</span><span class="sxs-lookup"><span data-stu-id="34daf-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="34daf-105">Registriredaktori abil Navigeerige HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="34daf-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="34daf-106">Kui DisableFileSyncNGSC on olemas ja see on seatud väärtusele 1, avage võti ja muutke väärtust väärtuseks 0.</span><span class="sxs-lookup"><span data-stu-id="34daf-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="34daf-107">OneDrive ' i käsitsi käivitamine, minnes avakuvale</span><span class="sxs-lookup"><span data-stu-id="34daf-107">Manually launch OneDrive by going to Start</span></span> ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="34daf-109">, tippige otsinguväljale sõna OneDrive ja seejärel klõpsake OneDrive ' i töölauarakenduse nuppu.</span><span class="sxs-lookup"><span data-stu-id="34daf-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="34daf-110">**OneDrive ' i lähtestamine.**</span><span class="sxs-lookup"><span data-stu-id="34daf-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="34daf-111">Märkmete</span><span class="sxs-lookup"><span data-stu-id="34daf-111">Notes:</span></span>

- <span data-ttu-id="34daf-112">OneDrive ' i lähtestamisel lahutatakse kõik teie olemasolevad sünkroonimise ühendused (sh teie isiklik OneDrive, kui olete häälestanud).</span><span class="sxs-lookup"><span data-stu-id="34daf-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="34daf-113">Te ei kaota faile ega andmeid, kui lähtestate OneDrive ' i oma arvutis.</span><span class="sxs-lookup"><span data-stu-id="34daf-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="34daf-114">**OneDrive ' i lähtestamiseks tehke järgmist.**</span><span class="sxs-lookup"><span data-stu-id="34daf-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="34daf-115">Dialoogiboksi Käivita avamiseks vajutage klahvikombinatsiooni Windowsi klahv ja R.</span><span class="sxs-lookup"><span data-stu-id="34daf-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="34daf-116">Tippige% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset ja vajutage nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="34daf-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="34daf-117">Käsuviiba aken võib olla lühike.</span><span class="sxs-lookup"><span data-stu-id="34daf-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="34daf-118">OneDrive ' i käsitsi käivitamine, minnes avakuvale</span><span class="sxs-lookup"><span data-stu-id="34daf-118">Manually launch OneDrive by going to Start</span></span> ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="34daf-120">, tippige otsinguväljale sõna OneDrive ja seejärel klõpsake OneDrive ' i töölauarakenduse nuppu.</span><span class="sxs-lookup"><span data-stu-id="34daf-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="34daf-121">Märkmete</span><span class="sxs-lookup"><span data-stu-id="34daf-121">Notes:</span></span>

- <span data-ttu-id="34daf-122">Kui olete enne lähtestamist valinud vaid mõne kausta sünkroonimise, peate seda uuesti tegema, kui sünkroonimine on lõpule viidud.</span><span class="sxs-lookup"><span data-stu-id="34daf-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="34daf-123">Lisateavet leiate teemast [OneDrive ' i kaustade valimine arvutiga sünkroonimiseks](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .</span><span class="sxs-lookup"><span data-stu-id="34daf-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="34daf-124">Peate selle täitma oma isikliku OneDrive ' i ja OneDrive for Businessi jaoks.</span><span class="sxs-lookup"><span data-stu-id="34daf-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>