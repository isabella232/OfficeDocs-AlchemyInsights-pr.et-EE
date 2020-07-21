---
title: Mitu kasutajat, kes ei näe Outlookis lisandmooduleid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197841"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="7a55f-102">Mitu kasutajat, kes ei näe Outlookis lisandmooduleid</span><span class="sxs-lookup"><span data-stu-id="7a55f-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="7a55f-103">Kui testite Outlooki lisandmoodulid ja ükski kuvatakse, esimese tõrkeotsingu samm, kasutage **cmdlet-käsu Get-OrganizationConfig** PowerShelli päringu _AppsForOfficeEnabled_ parameeter.</span><span class="sxs-lookup"><span data-stu-id="7a55f-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="7a55f-104">Kui päring tagastab väärtuse **False**, seadke selle parameetri **väärtuseks True** **set-OrganizationConfig cmdlet-käsu** abil, nii et lisandmoodulid kuvatakse ootuspäraselt.</span><span class="sxs-lookup"><span data-stu-id="7a55f-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="7a55f-105">Me ei soovita, et _AppsForOfficeEnabled_ parameeter on seatud **false**.</span><span class="sxs-lookup"><span data-stu-id="7a55f-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="7a55f-106">**Väär** väärtus alistab kõik ülaltoodud haldus- ja kasutajarollisätted ja takistab organisatsiooni mis tahes kasutaja aktiveerimist uute rakenduste poolt.</span><span class="sxs-lookup"><span data-stu-id="7a55f-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="7a55f-107">Lisateabe saamiseks vaadake teemat [Outlooki lisandmoodulite installimiseks ja haldamiseks administraatorite ja kasutajate määramine](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="7a55f-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>