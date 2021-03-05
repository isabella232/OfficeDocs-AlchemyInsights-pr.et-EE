---
title: Võrgu skannimine keelamine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481401"
---
# <a name="disable-network-scan"></a><span data-ttu-id="674d9-102">Võrgu skannimine keelamine</span><span class="sxs-lookup"><span data-stu-id="674d9-102">Disable network scan</span></span>

<span data-ttu-id="674d9-103">Võrgu ühiskasutuse skaneerimine võib mõjutada jõudlust.</span><span class="sxs-lookup"><span data-stu-id="674d9-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="674d9-104">Kui soovite tagada, et klient ei kontrolliks vaikimisi võrgu aktsiaid/faile, konfigureerige Windows Defenderi rakenduses **True** järgmised sätted.</span><span class="sxs-lookup"><span data-stu-id="674d9-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="674d9-105">DisableScanningMappedNetworkDrivesForFullScan</span><span class="sxs-lookup"><span data-stu-id="674d9-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="674d9-106">DisableScanningNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="674d9-106">DisableScanningNetworkFiles</span></span>