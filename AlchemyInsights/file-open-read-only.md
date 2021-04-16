---
title: Fail on avatud kirjutuskaitstuna
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813180"
---
# <a name="file-open-read-only"></a><span data-ttu-id="eff1f-102">Fail on avatud kirjutuskaitstuna</span><span class="sxs-lookup"><span data-stu-id="eff1f-102">File open read-only</span></span>

<span data-ttu-id="eff1f-103">Võimalik, et failide avamisel avatakse need kirjutuskaitstuna.</span><span class="sxs-lookup"><span data-stu-id="eff1f-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="eff1f-104">Mõnel juhul on see turvalisuse tagamiseks (nt failide avamisel Internetist) ja muudel aegadel võib põhjuseks olla säte, mida saab muuta.</span><span class="sxs-lookup"><span data-stu-id="eff1f-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="eff1f-105">Siin on mõned stsenaariumid, kus fail avaneb kirjutuskaitstuna, ja mõned toimingud, mida saate selle muutmiseks teha.</span><span class="sxs-lookup"><span data-stu-id="eff1f-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="eff1f-106">**Minu viirusetõrje põhjustab nende kirjutuskaitstud avamiseks**</span><span class="sxs-lookup"><span data-stu-id="eff1f-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="eff1f-107">Mõned viirusetõrjeprogrammid võivad teid kaitsta potentsiaalselt ebaturvaliste failide eest, avades need kirjutuskaitstuna.</span><span class="sxs-lookup"><span data-stu-id="eff1f-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="eff1f-108">Võimalik, et peate nende sätete kohandamise kohta teavet oma viirusetõrjeteenuse pakkujalt kontrollima.</span><span class="sxs-lookup"><span data-stu-id="eff1f-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="eff1f-109">BitDefender sisaldab näiteks sisu rakenduse välistamiste lisamise kohta siin: Rakenduse või protsessi välistamiste lisamine [Bitdefenderi juhtimiskeskuses.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="eff1f-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="eff1f-110">**Kas failia atribuudid on seatud kirjutuskaitstuks?**</span><span class="sxs-lookup"><span data-stu-id="eff1f-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="eff1f-111">Failiasuvaid atribuute saate kontrollida, paremklõpsades faili ja valides käsu Atribuudid.</span><span class="sxs-lookup"><span data-stu-id="eff1f-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="eff1f-112">Kui atribuut Kirjutuskaitstud on märgitud, saate selle tühjendada ja klõpsata nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="eff1f-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="eff1f-113">**Sisu on kaitstud vaates**</span><span class="sxs-lookup"><span data-stu-id="eff1f-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="eff1f-114">Internetist ja muudest potentsiaalselt ebaturvalistest asukohtadest pärit failid võivad sisaldada viirusi, ussviirusi või muud tüüpi ründevara, mis võivad teie arvutit kahjustada.</span><span class="sxs-lookup"><span data-stu-id="eff1f-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="eff1f-115">See kehtib tavaliselt ka meilimanuste või allalaaditud failide korral.</span><span class="sxs-lookup"><span data-stu-id="eff1f-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="eff1f-116">Arvuti kaitsmiseks avatakse kaitstud vaates failid nende potentsiaalselt ebaturvaliste asukohtade eest.</span><span class="sxs-lookup"><span data-stu-id="eff1f-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="eff1f-117">Kaitstud vaate abil saate lugeda faili ja vaadata selle sisu, vähendades samal ajal riske.</span><span class="sxs-lookup"><span data-stu-id="eff1f-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="eff1f-118">Lisateavet kaitstud vaate ja sätete muutmise kohta leiate sellest artiklist Mis on [kaitstud vaade?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="eff1f-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="eff1f-119">**Kas OneDrive on täis?**</span><span class="sxs-lookup"><span data-stu-id="eff1f-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="eff1f-120">Kui fail on salvestatud OneDrive'i ja teie OneDrive'i salvestusruum on täis, ei saa te dokumenti salvestada enne, kui olete eraldatud ruumi all.</span><span class="sxs-lookup"><span data-stu-id="eff1f-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="eff1f-121">Saate oneDrive'is vaba ruumi kontrollida, klõpsates teavituskeskuses OneDrive'i ikooni ja valides käsu Halda salvestusruumi või saate avada , sisse logida ja märkida ekraani vasakus allnurgas kasutatud [https://onedrive.live.com](https://onedrive.live.com) ruumi.</span><span class="sxs-lookup"><span data-stu-id="eff1f-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="eff1f-122">**Kas Office on aktiveeritud?**</span><span class="sxs-lookup"><span data-stu-id="eff1f-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="eff1f-123">Kui Office pole aktiveeritud või teie tellimus on aegunud, võite olla kirjutuskaitstud vähendatud funktsionaalsusega režiimis.</span><span class="sxs-lookup"><span data-stu-id="eff1f-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="eff1f-124">Lisateavet Office'i aktiveerimise kohta leiate teemast [Litsentsimata toote- ja aktiveerimistõrked Office's.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="eff1f-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="eff1f-125">**Kui kõik muu nurjub...**</span><span class="sxs-lookup"><span data-stu-id="eff1f-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="eff1f-126">Proovige arvuti taaskäivitada</span><span class="sxs-lookup"><span data-stu-id="eff1f-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="eff1f-127">Office'i värskenduste installimine</span><span class="sxs-lookup"><span data-stu-id="eff1f-127">Install Office updates</span></span>
    
- <span data-ttu-id="eff1f-128">Office'i parandamine võrgus</span><span class="sxs-lookup"><span data-stu-id="eff1f-128">Perform an Online repair of Office</span></span>
    

