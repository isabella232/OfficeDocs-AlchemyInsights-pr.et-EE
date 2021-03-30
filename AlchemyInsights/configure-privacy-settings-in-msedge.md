---
title: Microsoft Edge'is privaatsussätete konfigureerimine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404618"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="066f1-102">Microsoft Edge'is privaatsussätete konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="066f1-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="066f1-103">Kui Microsoft Edge on juurutatud mitte-Windowsi platvormidel, ei saadeta Microsoftile vaikimisi diagnostikaandmeid ega saiditeavet.</span><span class="sxs-lookup"><span data-stu-id="066f1-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="066f1-104">Kui Microsoft Edge on juurutatud opsüsteemis Windows 10, saadetakse diagnostikaandmed ja saiditeave vastavalt kasutajate [Windowsi diagnostikaandmete sätetele.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="066f1-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="066f1-105">Kui soovite konfigureerida, kuidas Microsoft Edge teie asutuse andmekogumist käsitleb, kasutage järgmisi rühmapoliitikaid.</span><span class="sxs-lookup"><span data-stu-id="066f1-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="066f1-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) lülitab sisse kasutuse ja krahhiga seotud andmete aruandluse.</span><span class="sxs-lookup"><span data-stu-id="066f1-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="066f1-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) saadab Microsofti teenuste täiustamiseks kasutatava saiditeabe.</span><span class="sxs-lookup"><span data-stu-id="066f1-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="066f1-108">Lisateavet leiate teemast [Poliitikasätete konfigureerimine.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="066f1-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
