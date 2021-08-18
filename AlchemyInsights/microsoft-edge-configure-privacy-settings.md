---
title: Microsoft Edge privaatsussätete konfigureerimine
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114168"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge privaatsussätete konfigureerimine

Vaikimisi, kui Microsoft Edge juurutatakse mitte-Windows, ei saadeta Microsoftile diagnostikaandmeid ega saiditeavet. Kui aga Microsoft Edge juurutatakse Windows 10, saadetakse diagnostikaandmed ja saiditeave vastavalt kasutajate [Windows diagnostikaandmete sätetele.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Ettevõtte Microsoft Edge andmete kogumise konfigureerimiseks kasutage järgmisi rühmapoliitikaid.
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): See poliitika võimaldab kasutusest ja krahhiga seotud andmetest teatamist.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): See poliitika saadab saiditeabe, mida kasutatakse Microsofti teenused.

Lisateavet leiate teemast [Poliitikasätete konfigureerimine.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)