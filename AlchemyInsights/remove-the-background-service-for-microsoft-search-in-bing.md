---
title: Microsoft Searchi taustapildi eemaldamine Bingis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816126"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Microsoft Searchi taustapildi eemaldamine Bingis

Bingis Microsoft Searchi taustapildi eemaldamiseks võite proovida järgmisi õiguskaitsevahendeid.

1. Algsete otsingumootori sätete taastamiseks tehke järgmist.

    loomine. Aktiveerige **Bingi kasutamine vaike-otsimootori [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)** väljalülitamiseks.

    b. [Avage Microsoft 365 halduskeskus](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ja tühjendage säte, mis mõjutab kõiki teie asutuse kasutajaid.

2. Kui soovite tausta teenuse üksikult seadmelt eemaldada, tehke järgmist.

    loomine. Valige Juhtpaneel **> programmid > programmid ja funktsioonid**.

    b. Paremklõpsake installitud programmide loendis jaotises **Microsoft Search (Bing** ) ja seejärel klõpsake käsku **desinstalli**.

3. Oma asutuse mitmest seadmest tausta teenuse eemaldamiseks logige sisse administraatorina ja käivitage skript järgmine käsk: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
