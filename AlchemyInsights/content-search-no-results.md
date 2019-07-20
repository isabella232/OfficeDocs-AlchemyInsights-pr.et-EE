---
title: Sisu otsida tulemeid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800298"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="8374c-102">Tulemeid: sisu otsing/eksport</span><span class="sxs-lookup"><span data-stu-id="8374c-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="8374c-103">Küsimused koos sisu otsing/eksport ei tule mingeid andmeid võib olla tingitud teatud konkreetsete Admin ja ei suhtle kõigile administraatoritel setup vastavuse turvalisusefiltrit.</span><span class="sxs-lookup"><span data-stu-id="8374c-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="8374c-104">Probleemi lahendamiseks kontrollige, kas täitmise turvalisuse filtreid, mis võivad põhjustada see:</span><span class="sxs-lookup"><span data-stu-id="8374c-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="8374c-105">Turvalisus ja vastavus Center PowerShelli ühendamine</span><span class="sxs-lookup"><span data-stu-id="8374c-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="8374c-106">Käivitage järgmine cmdlet-käsud:</span><span class="sxs-lookup"><span data-stu-id="8374c-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="8374c-107">$org = "teiedomeen.com"</span><span class="sxs-lookup"><span data-stu-id="8374c-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="8374c-108">Get-ComplianceSecurityFilter-organisatsiooni $org</span><span class="sxs-lookup"><span data-stu-id="8374c-108">Get-ComplianceSecurityFilter -Organization $org</span></span>