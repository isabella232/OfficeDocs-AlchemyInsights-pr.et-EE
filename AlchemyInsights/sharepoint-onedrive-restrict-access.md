---
title: Juurdepääsu piiramine SharePointis või OneDrive ' is
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700451"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Juurdepääsu piiramine SharePointis või OneDrive ' is

SharePoint Online ' i/OneDrive ' i teenustele juurdepääsu piiramiseks on mitu võimalust. Allpool on kirjeldatud järgmisi Accessi piirangute meetodeid. 

**Õiguste piirang**

SharePoint Online ' is ja OneDrive for Businessis piirame juurdepääsu sellistele üksustele nagu saidid, failid ja kaustad, võimaldades juurdepääsu ainult nendele rühmadele/isikutele, kellel on juurdepääs.

- [SharePointi loendi või teegi õiguse kohandamine](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePointi saidi kasutusõiguste kohandamine](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alamkausta õiguse muutmine](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Haldamata seadmetest juurdepääsu reguleerimine](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePointi või üldadministraatori saate hallata või piirata juurdepääsu SharePointi ja OneDrive ' i sisule haldamata seadmetest (need ei ole hübriid ad liitunud või ühilduvad Intune ' is).

**Võrgukoha piirang**

IT-administraatorina saate reguleerida juurdepääsu SharePointi ja OneDrive ' i ressurssidele, mis põhinevad teie usaldusväärsel võrgu asukohal. Seda tuntakse ka asukoha-põhise poliitikana. Lisateavet leiate teemast [SharePoint Online ' i ja OneDrive ' i andmetele juurdepääsu reguleerimine võrgu asukoha põhjal](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Saidi lukustuse piirang** 

SharePoint Online ' is saate saidikogumi lukustada, nii et keegi ei pääseks sellele juurde. See on määratud PowerShelli ja [SharePoint Online ' i halduse kesta](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kaudu, kasutades atribuuti [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Kasutajate ja alamsaitide loomise piiramine**

Kui olete SharePointi administraator või üldadministraator, saate lubada kasutajatel luua ja hallata oma SharePointi saite, määrata kindlaks, millist tüüpi saite nad saavad luua, ja määrata saitide asukoha. Lisateavet leiate teemast [saidi loomise haldamine SharePoint Online ' is](https://docs.microsoft.com/sharepoint/manage-site-creation)

