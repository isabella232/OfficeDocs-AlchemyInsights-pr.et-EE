---
title: Kas Teamsi klient jookseb kokku?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030587"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="394bd-102">Kas Teamsi klient jookseb kokku?</span><span class="sxs-lookup"><span data-stu-id="394bd-102">Teams client crashing?</span></span>

<span data-ttu-id="394bd-103">Kui teie Teamsi klient jookseb kokku, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="394bd-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="394bd-104">Kui kasutate Teamsi töölauarakendust, [veenduge, et rakendus oleks täielikult värskendatud](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="394bd-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="394bd-105">Veenduge, et kõik [Office 365 URL-id ja aadresside vahemikud](https://docs.microsoft.com/microsoftteams/connectivity-issues) oleksid juurdepääsetavad.</span><span class="sxs-lookup"><span data-stu-id="394bd-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="394bd-106">Logige oma administraatori kontoga sisse ja kontrollige oma [teenuse seisundi andmelauda](https://docs.microsoft.com/office365/enterprise/view-service-health), et teha kindlaks, kas ei esine katkestust ega teenuse jõudluse vähenemist.</span><span class="sxs-lookup"><span data-stu-id="394bd-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="394bd-107">Viimase toiminguna võite proovida tühjendada Teamsi kliendi vahemälu.</span><span class="sxs-lookup"><span data-stu-id="394bd-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="394bd-108">Väljuge täielikult Microsoft Teamsi töölauakliendist.</span><span class="sxs-lookup"><span data-stu-id="394bd-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="394bd-109">Saate paremklõpsata ikoonide alal **Teamsi** ja klõpsata suvandit **Sulge** või käivitada tegumihalduri ja protsessi täielikult sulgeda.</span><span class="sxs-lookup"><span data-stu-id="394bd-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="394bd-110">Minge File Explorerisse ja sisestage %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="394bd-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="394bd-111">Kataloogis kuvatakse üks järgmistest kaustadest.</span><span class="sxs-lookup"><span data-stu-id="394bd-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="394bd-112">Asukohas **Application Cache** (Rakenduse vahemälu) avage suvand Vahemälu ja kustutage kõik failid vahemälu asukohas: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="394bd-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="394bd-113">Kustutage asukohas **Blob_storage** (Bloobimälu) kõik failid: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="394bd-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="394bd-114">Kustutage asukohas **Cache** (Vahemälu) kõik failid: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="394bd-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="394bd-115">Kustutage asukohas **databases** (Andmebaasid) kõik failid: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="394bd-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="394bd-116">Kustutage asukohas **GPUCache** (GPU vahemälu) kõik failid: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="394bd-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="394bd-117">Kustutage asukohas **IndexedDB** (Indekseeritud DB) DB-fail: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="394bd-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="394bd-118">Kustutage asukohas **Local Storage** (Kohalik mälu) kõik failid: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="394bd-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="394bd-119">Viimasena kustutage asukohas **tmp** kõik failid: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="394bd-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="394bd-120">Taaskäivitage oma Teamsi klient.</span><span class="sxs-lookup"><span data-stu-id="394bd-120">Restart your Teams client.</span></span>
