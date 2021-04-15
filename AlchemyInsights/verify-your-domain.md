---
title: Domeeni kontrollimine
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770987"
---
# <a name="verify-your-domain"></a><span data-ttu-id="cda53-102">Domeeni kontrollimine</span><span class="sxs-lookup"><span data-stu-id="cda53-102">Verify your domain</span></span>

 <span data-ttu-id="cda53-103">**Kirjet pole arvatavasti kogu Interneti kaudu värskendatud.**</span><span class="sxs-lookup"><span data-stu-id="cda53-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="cda53-104">Tavaliselt kulub uue kirje vaatamiseks vaid paar minutit, kuid aeg-ajalt võib selleks aega võtta kuni paar tundi.</span><span class="sxs-lookup"><span data-stu-id="cda53-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="cda53-105">Kui olete nii kaua oodanud, kontrollige, kas olete kopeerinud ja kleepinud täpse väärtuse DNS-hostiteenuse pakkuja TXT-kinnituskirjesse.</span><span class="sxs-lookup"><span data-stu-id="cda53-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="cda53-106">Üks levinud probleem pole kirje "MS=" osa.</span><span class="sxs-lookup"><span data-stu-id="cda53-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="cda53-107">Meil on seda ka vaja!</span><span class="sxs-lookup"><span data-stu-id="cda53-107">We need that too!</span></span>

- <span data-ttu-id="cda53-108">Mõnel DNS-hostiteenuse pakkujal tuleb tsoonifaili (kus DNS-i kirje talletatakse) salvestamiseks teha lisateadmist, et see värskendatakse kogu Internetis.</span><span class="sxs-lookup"><span data-stu-id="cda53-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="cda53-109">Veenduge, et olete muudatused salvestanud, et Microsoft saaks kirjet vaadata ja kinnitada.</span><span class="sxs-lookup"><span data-stu-id="cda53-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
