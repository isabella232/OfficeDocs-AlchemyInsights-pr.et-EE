---
title: Drive shipping in the Microsoft 365 Import Service
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731442"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="d71d4-102">Drive shipping in the Microsoft 365 Import Service</span><span class="sxs-lookup"><span data-stu-id="d71d4-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="d71d4-103">Kasutage Drive'i saatmist, kopeerides PST-d kõvakettale ja seejärel saate kõvaketta Microsoftile.</span><span class="sxs-lookup"><span data-stu-id="d71d4-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="d71d4-104">Töö alustamiseks:</span><span class="sxs-lookup"><span data-stu-id="d71d4-104">To start the job:</span></span>

1. <span data-ttu-id="d71d4-105">Klõpsake Microsoft 365 Teabehaldus nuppu  **Impordi**.</span><span class="sxs-lookup"><span data-stu-id="d71d4-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="d71d4-106">Valige **Valige imporditöö tüüp** ja seejärel nupp **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="d71d4-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="d71d4-107">Selle impordi suvandi juhiste soovitud kohta soovitud importimiseks valige Käsk Saada kõvakettad ühte **meie füüsilistest asukohtadest.**</span><span class="sxs-lookup"><span data-stu-id="d71d4-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="d71d4-108">Siin on mõned asjad, mida meeles pidada.</span><span class="sxs-lookup"><span data-stu-id="d71d4-108">Here are some things to remember:</span></span>

- <span data-ttu-id="d71d4-109">PST-failide importimiseks postkasti postkasti Exchange Online postkastidele peab olema määratud Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d71d4-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="d71d4-110">Kui PST-d on suuremad kui 20 GB, võib jõudlus mõjutada jõudlust.</span><span class="sxs-lookup"><span data-stu-id="d71d4-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="d71d4-111">Toetatud on ainult 2,5-tollised tahkisdraivid (SSD-d) või 2,5- või 3,5-tollised SATA II/III sisemised kõvakettad.</span><span class="sxs-lookup"><span data-stu-id="d71d4-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="d71d4-112">PST-faile sisaldav kõvaketas peab olema krüptitud BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d71d4-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="d71d4-113">PST-failide importimiseks postkasti Microsoft 365 ketta kohaletoimetamise abil on $2 USD/GB andmete kohta.</span><span class="sxs-lookup"><span data-stu-id="d71d4-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="d71d4-114">Lisateavet PST-de importimiseks drive'i saatmisviisi kasutamise kohta leiate teemast Ketta saatmise kasutamine [ettevõtte PST-failide importimiseks.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="d71d4-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>