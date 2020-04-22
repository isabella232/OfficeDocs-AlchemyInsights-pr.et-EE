---
title: Juurdepääs on keelatud, kui vaatate töövoo
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687326"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="4a571-102">Juurdepääs on keelatud, kui vaatate töövoo</span><span class="sxs-lookup"><span data-stu-id="4a571-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="4a571-103">SharePoint 2013 töövoogude, mis üritavad saata e-posti SharePointi rühma võib nurjuda "juurdepääs keelatud" tõrketeade, kui SharePointi rühma liikmelisus on seatud kõigile.</span><span class="sxs-lookup"><span data-stu-id="4a571-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="4a571-104">**Selle probleemi lahendamiseks toimige järgmiselt.**</span><span class="sxs-lookup"><span data-stu-id="4a571-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="4a571-105">Lubage kõigil näha SharePointi rühma liikmeid.</span><span class="sxs-lookup"><span data-stu-id="4a571-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="4a571-106">Eemaldage SharePointi rühma e-posti rida to või CC.</span><span class="sxs-lookup"><span data-stu-id="4a571-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="4a571-107">Selgesõnaliselt lisada kasutajad to või CC rida, kui liikmelisus nähtavus ei saa muuta SharePointi rühma.</span><span class="sxs-lookup"><span data-stu-id="4a571-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="4a571-108">Lisateabe saamiseks vaadake [http volitamata/_vti_bin/Client.svc/SP.Utilities.Utility.sendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="4a571-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  