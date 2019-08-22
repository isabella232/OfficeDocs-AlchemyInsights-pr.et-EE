---
title: Piirata juurdepääsu SharePointi või OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559873"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Piirata juurdepääsu SharePointi või OneDrive

On palju võimalusi piirata juurdepääsu SharePoint Online/OneDrive teenuseid. Need erinevate juurdepääsu piiramise meetodid on toodud allpool. 

**Luba piirangut**

SharePoint Online ja OneDrive for Business, piirame juurdepääsu üksuste saidid, failid ja kaustad nende rühmade/isikute, kes peaks olema juurdepääs ainult andes.

- [Saate kohandada SharePointi loendi või teegi õiguste](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Saate kohandada SharePointi saidi õigused](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Muutke alamkausta õigusi](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kasutusõigus haldamata seadmed](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePointi või teenusekomplekti Office 365 globaalne admin, te saate blokeerida või SharePointis või OneDrive sisu piirata haldamata seadmetest (nende hübriid AD liidetud või ühilduv Intune).

**Võrgu asukoht piirang**

Nagu IT-administraator, saate kontrollida juurdepääsu SharePointis või OneDrive ressursse vastavalt kindlaksmääratud kohtades, mis on usaldusväärsed. See on ka asukohapõhised poliitika. Lisateabe saamiseks lugege [SharePoint Online ja OneDrive andmeid sõltuvalt juurdepääsu kontroll](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Saidipiirangut lukk** 

Jooksul SharePoint Online peate võime lukustada saidikogumi, nii et keegi ei ole juurdepääsu. See asub PowerShelli ja [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState atribuudi [SharePoint Online halduskesta](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kaudu.

**Piirata, saite või alamsaitide loomine**

SharePointi admin või Office 365 globaalne admin, võite oma kasutajad luua ja hallata oma SharePointi saitidele, kindlaks määrata, milliseid saite nad luua, ja määrake asukoht saidid. Lisateabe saamiseks lugege [SharePoint Online Halda saidi loomist](https://docs.microsoft.com/sharepoint/manage-site-creation)

