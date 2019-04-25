---
title: Kasutaja postkasti ümberarvestamisel ühiskasutuses postkasti?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374319"
---
<span data-ttu-id="933fb-102">Te saate teisendada ainult kasutaja postkasti ühiskasutuses postkasti kui kasutaja on Exchange litsents.</span><span class="sxs-lookup"><span data-stu-id="933fb-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="933fb-103">Pärast teisendamist postkasti, ta jätkab näidata aktiivselt sest detsembri ühiskasutuses olevad postkastid.</span><span class="sxs-lookup"><span data-stu-id="933fb-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="933fb-104">Siiski ümber postkasti ka kuvatakse loendis ühiskasutuses postkasti.</span><span class="sxs-lookup"><span data-stu-id="933fb-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="933fb-105">Kui proovite muuta postkasti Exchange konsoolis ja teisendus nurjub, tühjendage brauseri vahemälu ja küpsised ja proovige uuesti.</span><span class="sxs-lookup"><span data-stu-id="933fb-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="933fb-106">Kui see ikka ei tööta, proovige konverteeriva postkasti Exchange Management shelli poolt järgmise käsu:</span><span class="sxs-lookup"><span data-stu-id="933fb-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="933fb-107">Postkasti konverteerimise Lisateave on esitatud [muuta kasutaja postkasti ühiskasutuses postkasti](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="933fb-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
