---
title: Microsoft Edge ' i privaatsussätete konfigureerimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677251"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="f4251-102">Microsoft Edge ' i privaatsussätete konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="f4251-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="f4251-103">Kui Microsoft Edge on juurutatud mitte-Windowsi platvormidel, ei saadeta Microsoftile diagnostilisi andmeid ega saidi andmeid.</span><span class="sxs-lookup"><span data-stu-id="f4251-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="f4251-104">Kui Microsoft Edge on juurutatud opsüsteemis Windows 10, saadetakse diagnostilised andmed ja saidi teave vastavalt kasutajate [Windowsi diagnostiliste andmete sätetele](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="f4251-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="f4251-105">Kui soovite konfigureerida, kuidas Microsoft Edge teie asutuse andmete kogumist töötleb, kasutage järgmisi rühmapoliitika reegleid.</span><span class="sxs-lookup"><span data-stu-id="f4251-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="f4251-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): see poliitika võimaldab teavitada kasutus-ja krahhiga seotud andmetest.</span><span class="sxs-lookup"><span data-stu-id="f4251-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="f4251-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): see poliitika saadab Microsofti teenuste täiustamiseks kasutatava saidi teabe.</span><span class="sxs-lookup"><span data-stu-id="f4251-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="f4251-108">Lisateavet leiate teemast [poliitika sätete konfigureerimine](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="f4251-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>