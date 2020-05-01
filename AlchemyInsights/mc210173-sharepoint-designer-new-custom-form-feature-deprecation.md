---
title: MC210173 – SharePoint Designeri uue kohandatud vormi funktsiooni kasutuselt kõrvaldamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928524"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – SharePoint Designeri uue kohandatud vormi funktsiooni kasutuselt kõrvaldamine

Oleme tuvastanud probleemi, mis mõjutab SharePoint Online’is SharePoint Designeri funktsioone [kohandatud vormide loomisel](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2). Pärast hoolikat uurimist oleme teinud kindlaks, et sellele probleemile puudub teadaolev lahendus ja oleme otsustanud kohandatud vormi loomise funktsiooni alates laupäevast, 25. aprillist 2020 kl 3.00 keelata. See muudatus ei mõjuta võimalust redigeerida eelnevalt loodud vorme või teisi SharePoint Online Designeri olemasolevaid funktsioone.

Pärast selle muudatuse tegemist võidakse kasutajatele kuvada uue vormi looimsel tõrketeade „Loendi muudatusi ei saanud serverisse salvestada“.

Kasutajad, kes on varasemalt kasutanud kohandatud vormide loomiseks SharePoint Designerit, saavad nüüd sellel eesmärgil kasutada [PowerAppsi](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).

PowerApps on lihtne ja võimas tööriist, mis võimaldab SharePoint Online’i kaasaegset keskkonda kasutavatel kasutajatel luua ja redigeerida SharePointi loendite kohandatud vorme ja dokumendi teeke otse brauseriaknast. PowerApps ei vaja traditsioonilist kodeerimise teadmist ega ühtegi täiendavat rakenduse allalaadimist (nt InfoPath).

**Märkus.**. Klassikalise SharePoint Online’i kasutajad peavad ajutiselt vahetama kaasaegsele keskkonnale, et pääseda ligi ja kasutada rakendust PowerApps. Samas on kõik PowerAppsis loodud kohandatud vormid klassikalise SharePoint Online’i keskkonna kasutajatele kättesaadavad.
