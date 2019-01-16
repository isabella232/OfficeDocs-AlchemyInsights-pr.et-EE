---
title: 1554 Winsock-tõrge 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28285272"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="a3b82-102">Winsocki tõrge 10061</span><span class="sxs-lookup"><span data-stu-id="a3b82-102">Winsock error 10061</span></span>

<span data-ttu-id="a3b82-p101">See tähendab, et Office 365 ei saanud luua TCP pesa (ühendus) Sihthosti. Selle tõrke põhjuseks enamasti oma tulemüüri konfiguratsiooni osas probleemi. Probleemi lahendamiseks kontrollige neid sätteid:</span><span class="sxs-lookup"><span data-stu-id="a3b82-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="a3b82-106">Kontrollige oma tulemüüri konfiguratsiooni teabe [Office 365 URL-id](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) ja IP-aadressid</span><span class="sxs-lookup"><span data-stu-id="a3b82-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="a3b82-107">Kui viga ilmneb et Exchange Online kaitse (EOP), sa peaks on varem teatatud muudatusi [Exchange Online kaitse IP-aadressid](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="a3b82-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="a3b82-108">Veenduge, et teie Interneti-teenuse pakkuja (ISP) ei blokeeri sadama.</span><span class="sxs-lookup"><span data-stu-id="a3b82-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="a3b82-109">Nutika hosti ja sihtarvutite serveri sätteid oma pistikud kontrollida.</span><span class="sxs-lookup"><span data-stu-id="a3b82-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="a3b82-110">Pange tähele, et Office 365 ei blokeerida *sissetulevad* ühendused sel viisil.</span><span class="sxs-lookup"><span data-stu-id="a3b82-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

