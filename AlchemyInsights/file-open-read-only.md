---
title: Fail on avatud kirjutuskaitstud
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: c045188af15fcec0f868eb0e5b399bd1fb42a09a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702770"
---
# <a name="file-open-read-only"></a><span data-ttu-id="56e4f-102">Fail on avatud kirjutuskaitstud</span><span class="sxs-lookup"><span data-stu-id="56e4f-102">File open read-only</span></span>

<span data-ttu-id="56e4f-103">Võite leida, et failide avamisel avatakse need kirjutuskaitstutena.</span><span class="sxs-lookup"><span data-stu-id="56e4f-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="56e4f-104">Mõnel juhul on see lisatud turvalisuse jaoks, näiteks failide avamisel Internetist ja muul ajal võib see olla tingitud seadistusest, mida saab muuta.</span><span class="sxs-lookup"><span data-stu-id="56e4f-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="56e4f-105">Siin on mõned stsenaariumid, kus fail avab kirjutuskaitstud ja mõned sammud, mida saate teha, et seda muuta.</span><span class="sxs-lookup"><span data-stu-id="56e4f-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="56e4f-106">**Minu viirusetõrje põhjustab neid avada kirjutuskaitstud**</span><span class="sxs-lookup"><span data-stu-id="56e4f-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="56e4f-107">Mõned viirusetõrjeprogrammid võivad teid potentsiaalselt ebaturvaliste failide eest kaitsta, avades need kirjutuskaitstuna.</span><span class="sxs-lookup"><span data-stu-id="56e4f-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="56e4f-108">Teil võib olla vaja kontrollida oma viirusetõrje pakkuja teada, kuidas reguleerida neid seadeid.</span><span class="sxs-lookup"><span data-stu-id="56e4f-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="56e4f-109">Näiteks BitDefender on sisu lisamine rakenduse erandid siin: [Kuidas lisada rakenduse või protsessi väljaarvamisi Bitdefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="56e4f-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="56e4f-110">**Kas failiatribuudid on seatud kirjutuskaitstud?**</span><span class="sxs-lookup"><span data-stu-id="56e4f-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="56e4f-111">Faili atribuute saate kontrollida paremklõpsates failil ja valides atribuudid.</span><span class="sxs-lookup"><span data-stu-id="56e4f-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="56e4f-112">Kui kirjutuskaitstud atribuut on märgitud, võite selle tühjendada ja klõpsata nuppu OK.</span><span class="sxs-lookup"><span data-stu-id="56e4f-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="56e4f-113">**Sisu on kaitstud vaates**</span><span class="sxs-lookup"><span data-stu-id="56e4f-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="56e4f-114">Internetist ja muudest potentsiaalselt ebaturvalistest kohtadest pärit failid võivad sisaldada viirusi, usside või muud tüüpi õelvara, mis võib teie arvutit kahjustada.</span><span class="sxs-lookup"><span data-stu-id="56e4f-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="56e4f-115">See on tavaliselt ka meilimanuste või allalaaditud failide puhul.</span><span class="sxs-lookup"><span data-stu-id="56e4f-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="56e4f-116">Teie arvuti kaitsmiseks avatakse nende potentsiaalselt ebaturvaliste asukohtade failid kaitstud vaates.</span><span class="sxs-lookup"><span data-stu-id="56e4f-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="56e4f-117">Kaitstud vaate abil saate lugeda faili ja vaadata selle sisu, vähendades samal ajal riske.</span><span class="sxs-lookup"><span data-stu-id="56e4f-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="56e4f-118">Kaitstud vaate ja sätete muutmise kohta lisateabe saamiseks lugege käesoleva artikli: [mis on kaitstud vaade?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="56e4f-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="56e4f-119">**Kas OneDrive on täis?**</span><span class="sxs-lookup"><span data-stu-id="56e4f-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="56e4f-120">Kui fail on talletatud OneDrive ' is ja teie OneDrive ' i salvestusruum on täis, ei saa te dokumenti salvestada enne, kui olete määratud ruumi all.</span><span class="sxs-lookup"><span data-stu-id="56e4f-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="56e4f-121">Võite kontrollida oma vaba ruumi OneDrive ' is, klõpsates teatiskeskuses asuvat OneDrive ' i ikooni ja valides salvestusruumi haldamine, või võite minna [https://onedrive.live.com](https://onedrive.live.com), logige sisse ja märkige ekraani alumises vasakus osas kasutatud ruumi hulk.</span><span class="sxs-lookup"><span data-stu-id="56e4f-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="56e4f-122">**Kas Office on aktiveeritud?**</span><span class="sxs-lookup"><span data-stu-id="56e4f-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="56e4f-123">Kui Office ei ole aktiveeritud või kui teie tellimus on aegunud, võite olla kirjutuskaitstud vähendatud funktsionaalsusega režiimis.</span><span class="sxs-lookup"><span data-stu-id="56e4f-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="56e4f-124">Office ' i aktiveerimise kohta leiate teavet teemast: [litsentsimata toote-ja aktiveerimistõrked](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="56e4f-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="56e4f-125">**Kui kõik muu ebaõnnestub...**</span><span class="sxs-lookup"><span data-stu-id="56e4f-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="56e4f-126">Taaskäivitage arvuti</span><span class="sxs-lookup"><span data-stu-id="56e4f-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="56e4f-127">Office ' i värskenduste installimine</span><span class="sxs-lookup"><span data-stu-id="56e4f-127">Install Office updates</span></span>
    
- <span data-ttu-id="56e4f-128">Office ' i võrguparanduse teostamine</span><span class="sxs-lookup"><span data-stu-id="56e4f-128">Perform an Online repair of Office</span></span>
    

