---
title: Kontrollige oma domeeni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d37cdae616fabd2813dc7c8074e94b05f0391d20
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29466854"
---
# <a name="verify-your-domain"></a><span data-ttu-id="35ca4-102">Kontrollige oma domeeni</span><span class="sxs-lookup"><span data-stu-id="35ca4-102">Verify your domain</span></span>

 <span data-ttu-id="35ca4-103">**Kirje pole ilmselt värskendada Interneti.**</span><span class="sxs-lookup"><span data-stu-id="35ca4-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="35ca4-104">Tavaliselt kulub vaid paar minutit meile vaadata uue kirje, kuid vahel võib võtta aega kuni paar tundi.</span><span class="sxs-lookup"><span data-stu-id="35ca4-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="35ca4-p101">Kui see on juba ammu oodanud, kontrollige üle, et te olete kopeerimisel ja kleepimisel TXT Taatlusprotokolli täpne väärtus kell DNS host. Üks levinud küsimus on ka selle "MS =" osa kirje. Seda on vaja liiga!</span><span class="sxs-lookup"><span data-stu-id="35ca4-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="35ca4-p102">Mõned DNS hosts, pead võtma lisatööd (DNS-kirje salvestamise) tsooni faili salvestamiseks nii, et see update Internetis. Veenduge, et salvestate muudatused nii Office 365 näete ja kirje.</span><span class="sxs-lookup"><span data-stu-id="35ca4-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

