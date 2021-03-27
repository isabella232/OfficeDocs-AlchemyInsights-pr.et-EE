---
title: Microsoft Edge'i käsitsi sisselogimine
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398653"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Microsoft Edge'i käsitsi sisselogimine

Kui kasutaja ei ole esimese kasutuskogemuse ajal automaatselt sisse logitud, saab kasutaja brauseri sätete või identiteedi hüpiku kaudu käsitsi sisse logida. Sisselogimise haldamiseks kasutage järgmisi poliitikaid.

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – tagamaks, et kasutajal on Microsoft Edge'is alati tööprofiil.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – sisselogimise piiramiseks usaldusväärsete kontodega.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – sisselogimise keelamiseks või kasutajate sisse logimiseks.

