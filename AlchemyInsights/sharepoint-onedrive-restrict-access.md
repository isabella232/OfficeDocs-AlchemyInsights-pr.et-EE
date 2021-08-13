---
title: Juurdepääsu piiramine SharePoint või OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093816"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Juurdepääsu piiramine SharePoint või OneDrive

Veebi- ja SharePoint teenustele juurdepääsu piiramiseks on OneDrive võimalusi. Allpool on kirjeldatud järgmisi juurdepääsupiirangute meetodeid. 

**Õigusepiirang**

Veebi SharePoint ja OneDrive for Business piirame juurdepääsu üksustele (nt saitidele, failidele ja kaustadele), andes juurdepääsu ainult nendele rühmadele/üksikisikutele, kellel peaks olema juurdepääs.

- [Loendi või teegi SharePoint õiguste kohandamine](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Saidi SharePoint kohandamine](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alamkausta õiguste muutmine](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Mittehallatavatest seadmetest juurdepääsu reguleerimine](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint või üldadministraatorina saate blokeerida või piirata juurdepääsu mittehallatud seadmete SharePoint ja OneDrive sisule (need, mis pole Intune'i hübriid-AD-ga ühendatud või ühilduvad).

**Võrguasukoha piirang**

IT-administraatorina saate määrata juurdepääsu SharePoint ja OneDrive määratud võrgukohtadele, mida usaldate. Seda nimetatakse ka asukohapõhiseks poliitikaks. Lisateavet leiate teemast SharePoint [Online'i ja OneDrive juurdepääsu juhtimine võrguasukoha põhjal](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Saidi lukustamise piirang** 

Veebi SharePoint on teil võimalus saidikogumi lukustada, et keegi ei pääseks juurde. See on määratud PowerShelli ja [SharePoint Online Management Shelli](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kaudu atribuudi [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState abil.

**Kasutajate saitide või alamsaitide loomise piiramine**

Administraatorina SharePoint üldadministraatorina saate lasta kasutajatel luua ja hallata oma SharePoint saite, määrata, milliseid saite nad luua saavad, ja määrata saitide asukoha. Lisateavet leiate teemast Saidi [loomise haldamine SharePoint Online'is](https://docs.microsoft.com/sharepoint/manage-site-creation)

