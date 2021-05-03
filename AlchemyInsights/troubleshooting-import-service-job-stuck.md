---
title: Teenuse imporditöö tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125107"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="19e99-102">Teenuse imporditöö tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="19e99-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="19e99-103">Kui teil on probleeme teenuse imporditöödega, mis on kinni jäänud või nurjunud, uurige ja proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="19e99-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="19e99-104">Vaadake ÜLE PST-faili maht.</span><span class="sxs-lookup"><span data-stu-id="19e99-104">Review the size of of the PST file.</span></span> <span data-ttu-id="19e99-105">Pst-faili maksimaalne soovitatav maht importimiseks on 20 GB.</span><span class="sxs-lookup"><span data-stu-id="19e99-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="19e99-106">Kui kahtlustate, et üksused on rikutud, käivitage Scanpst.exe ja parandage TÕRKED PST-failides.</span><span class="sxs-lookup"><span data-stu-id="19e99-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="19e99-107">Kui importimisel kuvatakse tõrketeade "MapiExceptionShutoffQuotaExceeded" (MapiExceptionShutoffQuotaExceeded), veenduge, et sihtpostkastil oleks soovitud PST-failide importimiseks piisavalt võimsust.</span><span class="sxs-lookup"><span data-stu-id="19e99-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="19e99-108">LISATEAVET PST-imporditöö probleemide tõrkeotsingu kohta leiate teemast [PST-imporditöödega seotud probleemide tõrkeotsing.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="19e99-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="19e99-109">Lisateavet pst-ide importimisel Outlook leiate teemast PST Outlook-faili [(microsoft.com) importimisega](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)seotud probleemide lahendamine.</span><span class="sxs-lookup"><span data-stu-id="19e99-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>