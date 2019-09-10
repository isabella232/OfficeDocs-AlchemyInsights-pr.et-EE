---
title: Fail on avatud kirjutuskaitstud
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822230"
---
# <a name="file-open-read-only"></a><span data-ttu-id="69853-102">Fail on avatud kirjutuskaitstud</span><span class="sxs-lookup"><span data-stu-id="69853-102">File open read-only</span></span>

<span data-ttu-id="69853-103">Võite leida, et failide avamisel avatakse need kirjutuskaitstutena.</span><span class="sxs-lookup"><span data-stu-id="69853-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="69853-104">Mõnel juhul on see lisatud turvalisuse jaoks, näiteks failide avamisel Internetist ja muul ajal võib see olla tingitud seadistusest, mida saab muuta.</span><span class="sxs-lookup"><span data-stu-id="69853-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="69853-105">Siin on mõned stsenaariumid, kus fail avab kirjutuskaitstud ja mõned sammud, mida saate teha, et seda muuta.</span><span class="sxs-lookup"><span data-stu-id="69853-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="69853-106">**Minu viirusetõrje põhjustab neid avada kirjutuskaitstud**</span><span class="sxs-lookup"><span data-stu-id="69853-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="69853-107">Mõned viirusetõrjeprogrammid võivad teid potentsiaalselt ebaturvaliste failide eest kaitsta, avades need kirjutuskaitstuna.</span><span class="sxs-lookup"><span data-stu-id="69853-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="69853-108">Teil võib olla vaja kontrollida oma viirusetõrje pakkuja teada, kuidas reguleerida neid seadeid.</span><span class="sxs-lookup"><span data-stu-id="69853-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="69853-109">Näiteks BitDefender on sisu lisamine rakenduse erandid siin: [Kuidas lisada rakenduse või protsessi väljaarvamisi Bitdefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="69853-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="69853-110">**Kas failiatribuudid on seatud kirjutuskaitstud?**</span><span class="sxs-lookup"><span data-stu-id="69853-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="69853-111">Faili atribuute saate kontrollida paremklõpsates failil ja valides atribuudid.</span><span class="sxs-lookup"><span data-stu-id="69853-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="69853-112">Kui kirjutuskaitstud atribuut on märgitud, võite selle tühjendada ja klõpsata nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="69853-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="69853-113">**Sisu on kaitstud vaates**</span><span class="sxs-lookup"><span data-stu-id="69853-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="69853-114">Internetist ja muudest potentsiaalselt ebaturvalistest kohtadest pärit failid võivad sisaldada viirusi, usside või muud tüüpi õelvara, mis võib teie arvutit kahjustada.</span><span class="sxs-lookup"><span data-stu-id="69853-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="69853-115">See on tavaliselt ka meilimanuste või allalaaditud failide puhul.</span><span class="sxs-lookup"><span data-stu-id="69853-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="69853-116">Teie arvuti kaitsmiseks avatakse nende potentsiaalselt ebaturvaliste asukohtade failid kaitstud vaates.</span><span class="sxs-lookup"><span data-stu-id="69853-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="69853-117">Kaitstud vaate abil saate lugeda faili ja vaadata selle sisu, vähendades samal ajal riske.</span><span class="sxs-lookup"><span data-stu-id="69853-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="69853-118">Kaitstud vaate ja sätete muutmise kohta lisateabe saamiseks lugege käesoleva artikli: [mis on kaitstud vaade?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="69853-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="69853-119">**Kas OneDrive on täis?**</span><span class="sxs-lookup"><span data-stu-id="69853-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="69853-120">Kui fail on talletatud OneDrive ' is ja teie OneDrive ' i salvestusruum on täis, ei saa te dokumenti salvestada enne, kui olete määratud ruumi all.</span><span class="sxs-lookup"><span data-stu-id="69853-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="69853-121">Võite kontrollida oma vaba ruumi OneDrive ' is, klõpsates teatiskeskuses asuvat OneDrive ' i ikooni ja valides salvestusruumi haldamine, või võite minna [http://onedrive.live.com](http://onedrive.live.com), logige sisse ja märkige ekraani alumises vasakus osas kasutatud ruumi hulk.</span><span class="sxs-lookup"><span data-stu-id="69853-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="69853-122">**Kas Office on aktiveeritud?**</span><span class="sxs-lookup"><span data-stu-id="69853-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="69853-123">Kui Office ei ole aktiveeritud või kui teie tellimus on aegunud, võite olla kirjutuskaitstud vähendatud funktsionaalsusega režiimis.</span><span class="sxs-lookup"><span data-stu-id="69853-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="69853-124">Office ' i aktiveerimise kohta leiate teavet teemast: [litsentsimata toote-ja aktiveerimistõrked](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="69853-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="69853-125">**Kui kõik muu ebaõnnestub...**</span><span class="sxs-lookup"><span data-stu-id="69853-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="69853-126">Taaskäivitage arvuti</span><span class="sxs-lookup"><span data-stu-id="69853-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="69853-127">Office ' i värskenduste installimine</span><span class="sxs-lookup"><span data-stu-id="69853-127">Install Office updates</span></span>
    
- <span data-ttu-id="69853-128">Office ' i võrguparanduse teostamine</span><span class="sxs-lookup"><span data-stu-id="69853-128">Perform an Online repair of Office</span></span>
    

