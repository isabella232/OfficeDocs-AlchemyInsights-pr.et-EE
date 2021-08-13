---
title: Tundlikkussiltide piirangud Office failide SharePoint ja OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813153"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Tundlikkussiltide piirangud Office failide SharePoint ja OneDrive

Kui lubate tundlikkussildid Office failidele SharePoint ja OneDrive, olge teadlik nõuetest ja piirangutest, mis hõlmavad järgmist.

- SharePoint ja OneDrive ei saa töödelda faile, mis on sildistatud ja krüptitud Office töölauarakendustest, kui failid sisaldavad PowerQuery andmeid, kohandatud lisandmoodulite salvestatud andmeid või kohandatud XML-osi.
- SharePoint ja OneDrive ei rakenda tundlikkussilte automaatselt olemasolevatele failidele, mille olete juba Azure'i teabekaitse (AIP) siltide abil krüptitud. Tundlikkussiltide rakendamiseks krüptitud failidele: 
    - Veenduge, et AIP-sildid on migreeritud ja avaldatud Microsoft 365 vastavuskeskusesse.
    - Laadige sildistatud failid alla ja laadige need seejärel üles nende algsesse SharePoint või OneDrive asukohta.
- Krüptitud dokumentide puhul ei toetata printimist.

Lisateavet piirangute kohta leiate teemast Office ja [SharePoint](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)OneDrive .
