---
title: MC210173 – SharePoint Designeri uue kohandatud vormi funktsiooni kasutuselt kõrvaldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831802"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – SharePoint Designeri uue kohandatud vormi funktsiooni kasutuselt kõrvaldamine

Oleme tuvastanud probleemi, mis mõjutab SharePoint Online’is SharePoint Designeri funktsioone [kohandatud vormide loomisel](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2). Pärast hoolikat uurimist oleme teinud kindlaks, et sellele probleemile puudub teadaolev lahendus ja oleme otsustanud kohandatud vormi loomise funktsiooni alates laupäevast, 25. aprillist 2020 kl 3.00 keelata. See muudatus ei mõjuta võimalust redigeerida eelnevalt loodud vorme või teisi SharePoint Online Designeri olemasolevaid funktsioone.

Pärast selle muudatuse tegemist võidakse kasutajatele kuvada uue vormi looimsel tõrketeade „Loendi muudatusi ei saanud serverisse salvestada“.

Kasutajad, kes on varasemalt kasutanud kohandatud vormide loomiseks SharePoint Designerit, saavad nüüd sellel eesmärgil kasutada [PowerAppsi](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).

PowerApps on lihtne ja võimas tööriist, mis võimaldab SharePoint Online’i kaasaegset keskkonda kasutavatel kasutajatel luua ja redigeerida SharePointi loendite kohandatud vorme ja dokumendi teeke otse brauseriaknast. PowerApps ei vaja traditsioonilist kodeerimise teadmist ega ühtegi täiendavat rakenduse allalaadimist (nt InfoPath).

**Märkus.**. Klassikalise SharePoint Online’i kasutajad peavad ajutiselt vahetama kaasaegsele keskkonnale, et pääseda ligi ja kasutada rakendust PowerApps. Samas on kõik PowerAppsis loodud kohandatud vormid klassikalise SharePoint Online’i keskkonna kasutajatele kättesaadavad.
