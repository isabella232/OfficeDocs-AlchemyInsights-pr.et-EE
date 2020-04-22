---
title: SharePointi või OneDrive ' i juurdepääsu piiramine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692761"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePointi või OneDrive ' i juurdepääsu piiramine

On palju viise, kuidas piirata juurdepääsu SharePoint Online/OneDrive teenused. Need erinevad juurdepääsupiirangu meetodid on toodud allpool. 

**Õiguste piirang**

SharePoint Online ' i ja OneDrive for Business, piirame juurdepääsu üksustele nagu saidid, failid ja kaustad, ainult andes juurdepääsu neile rühmadele/isikutele, kellel peaks olema juurdepääs.

- [SharePointi loendi või teegi õiguste kohandamine](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePointi saidiga õiguste kohandamine](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alamkausta õiguste muutmine](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Haldamata seadmete juurdepääsu kontrollimine](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePointi või globaalse admin, saate blokeerida või piirata juurdepääsu SharePointi ja OneDrive ' i sisu haldamata seadmete (need ei ole hübriid AD liidetud või ühilduv Intune).

**Võrguasukoha piirang**

IT-administraatoriks saate reguleerida juurdepääsu SharePointi ja OneDrive ' i ressurssidele, mis põhinevad määratletud võrguasukohtadele, mida te usaldate. Seda nimetatakse ka asukohapõhise poliitika. Lisateabe saamiseks vaadake [juurdepääsu SharePoint Online ' i ja OneDrive andmed võrgu asukoha järgi](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Saidideluku piirang** 

SharePoint Online ' i sees on teil võimalus saidikogumi lukustada, nii et keegi ei pääse juurde. See on seatud PowerShelli ja [SharePoint Online Management shelli](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) abil [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate atribuut.

**Kasutajate piiramine saitide või alamsaitide loomisega**

SharePointi administraatori või globaalse administraatoriks saate lasta oma kasutajatel luua ja hallata oma SharePointi saite, määratleda, milliseid saite nad saavad luua, ja määrata saitide asukoha. Lisateabe saamiseks lugege [saidi loomine SharePoint Online ' i haldamine](https://docs.microsoft.com/sharepoint/manage-site-creation)

