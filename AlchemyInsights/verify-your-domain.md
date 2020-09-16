---
title: Domeeni kinnitamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734302"
---
# <a name="verify-your-domain"></a><span data-ttu-id="171cf-102">Domeeni kinnitamine</span><span class="sxs-lookup"><span data-stu-id="171cf-102">Verify your domain</span></span>

 <span data-ttu-id="171cf-103">**Kirje pole arvatavasti Internetis värskendatud.**</span><span class="sxs-lookup"><span data-stu-id="171cf-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="171cf-104">See võtab tavaliselt aega vaid mõne minuti, et saaksime uut kirjet näha, kuid mõnikord võib see kesta mõne tunni.</span><span class="sxs-lookup"><span data-stu-id="171cf-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="171cf-105">Kui olete juba ammu oodanud, kontrollige, kas olete kopeerinud ja kleepinud täpse väärtuse teie DNS-i hosti TXT-verifitseerimise kirjele.</span><span class="sxs-lookup"><span data-stu-id="171cf-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="171cf-106">Ühe levinud probleem ei sisalda kirje osa "MS =".</span><span class="sxs-lookup"><span data-stu-id="171cf-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="171cf-107">Meil on seda ka vaja!</span><span class="sxs-lookup"><span data-stu-id="171cf-107">We need that too!</span></span>

- <span data-ttu-id="171cf-108">Teatud DNS-i hostide korral peate tsooni faili (kus DNS-i kirje talletatud) salvestamiseks tegema täiendava toimingu, et see värskendatakse üle Interneti.</span><span class="sxs-lookup"><span data-stu-id="171cf-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="171cf-109">Veenduge, et olete muudatused salvestanud, et Microsoft saaks kirjet vaadata ja kinnitada.</span><span class="sxs-lookup"><span data-stu-id="171cf-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
