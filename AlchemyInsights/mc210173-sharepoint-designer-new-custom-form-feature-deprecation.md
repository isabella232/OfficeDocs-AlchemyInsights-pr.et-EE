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
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="60182-102">MC210173 – SharePoint Designeri uue kohandatud vormi funktsiooni kasutuselt kõrvaldamine</span><span class="sxs-lookup"><span data-stu-id="60182-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="60182-103">Oleme tuvastanud probleemi, mis mõjutab SharePoint Online’is SharePoint Designeri funktsioone [kohandatud vormide loomisel](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2).</span><span class="sxs-lookup"><span data-stu-id="60182-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="60182-104">Pärast hoolikat uurimist oleme teinud kindlaks, et sellele probleemile puudub teadaolev lahendus ja oleme otsustanud kohandatud vormi loomise funktsiooni alates laupäevast, 25. aprillist 2020 kl 3.00 keelata.</span><span class="sxs-lookup"><span data-stu-id="60182-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="60182-105">See muudatus ei mõjuta võimalust redigeerida eelnevalt loodud vorme või teisi SharePoint Online Designeri olemasolevaid funktsioone.</span><span class="sxs-lookup"><span data-stu-id="60182-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="60182-106">Pärast selle muudatuse tegemist võidakse kasutajatele kuvada uue vormi looimsel tõrketeade „Loendi muudatusi ei saanud serverisse salvestada“.</span><span class="sxs-lookup"><span data-stu-id="60182-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="60182-107">Kasutajad, kes on varasemalt kasutanud kohandatud vormide loomiseks SharePoint Designerit, saavad nüüd sellel eesmärgil kasutada [PowerAppsi](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="60182-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="60182-108">PowerApps on lihtne ja võimas tööriist, mis võimaldab SharePoint Online’i kaasaegset keskkonda kasutavatel kasutajatel luua ja redigeerida SharePointi loendite kohandatud vorme ja dokumendi teeke otse brauseriaknast.</span><span class="sxs-lookup"><span data-stu-id="60182-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="60182-109">PowerApps ei vaja traditsioonilist kodeerimise teadmist ega ühtegi täiendavat rakenduse allalaadimist (nt InfoPath).</span><span class="sxs-lookup"><span data-stu-id="60182-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="60182-110">**Märkus.**. Klassikalise SharePoint Online’i kasutajad peavad ajutiselt vahetama kaasaegsele keskkonnale, et pääseda ligi ja kasutada rakendust PowerApps. Samas on kõik PowerAppsis loodud kohandatud vormid klassikalise SharePoint Online’i keskkonna kasutajatele kättesaadavad.</span><span class="sxs-lookup"><span data-stu-id="60182-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
