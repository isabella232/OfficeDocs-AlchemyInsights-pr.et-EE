---
title: SharePointi või OneDrive ' i juurdepääsu piiramine
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750660"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePointi või OneDrive ' i juurdepääsu piiramine

On palju viise, kuidas piirata juurdepääsu SharePoint Online/OneDrive teenused. Need erinevad juurdepääsupiirangu meetodid on toodud allpool. 

**Õiguste piirang**

SharePoint Online ' i ja OneDrive for Business, piirame juurdepääsu üksustele nagu saidid, failid ja kaustad, ainult andes juurdepääsu neile rühmadele/isikutele, kellel peaks olema juurdepääs.

- [SharePointi loendi või teegi õiguste kohandamine](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePointi saidiga õiguste kohandamine](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alamkausta õiguste muutmine](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Haldamata seadmete juurdepääsu kontrollimine](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePointi või globaalse admin Office 365, saate blokeerida või piirata juurdepääsu SharePointi ja OneDrive ' i sisu haldamata seadmete (need ei ole hübriid AD ühendatud või Intune).

**Võrguasukoha piirang**

IT-administraatoriks saate reguleerida juurdepääsu SharePointi ja OneDrive ' i ressurssidele, mis põhinevad määratletud võrguasukohtadele, mida te usaldate. Seda nimetatakse ka asukohapõhise poliitika. Lisateabe saamiseks vaadake [juurdepääsu SharePoint Online ' i ja OneDrive andmed võrgu asukoha järgi](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Saidideluku piirang** 

SharePoint Online ' i sees on teil võimalus saidikogumi lukustada, nii et keegi ei pääse juurde. See on seatud PowerShelli ja [SharePoint Online Management shelli](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) abil [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate atribuut.

**Kasutajate piiramine saitide või alamsaitide loomisega**

SharePointi administraator või Office 365 globaalse admin, saate lasta oma kasutajatel luua ja hallata oma SharePointi saite, määratleda, milliseid saite nad saavad luua ja määrata saitide asukoht. Lisateabe saamiseks lugege [saidi loomine SharePoint Online ' i haldamine](https://docs.microsoft.com/sharepoint/manage-site-creation)

