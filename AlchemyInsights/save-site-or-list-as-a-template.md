---
title: Saidi või loendi salvestamine mallina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048720"
---
# <a name="save-site-or-list-as-a-template"></a>Saidi või loendi salvestamine mallina

SharePointi saidimallid on eelehitatud määratlused, mis on mõeldud konkreetse ärivajaduse ümber. Lisateavet leiate jaotisest [mallide kasutamine erinevat tüüpi SharePointi saitide loomiseks](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Siin on mõned levinud probleemid/lahendused saidi või loendi salvestamisel mallina SharePoint Online ' is.

**Saidi/loendimalli nupu salvestamine pole saadaval või puudub**. 

- Administraatorid peavad lubama kohandatud skripti malli funktsioonide lubamiseks. Üksikasjalikke juhiseid, näiteid ja kaalutlusi vt [kohandatud skripti lubamine või vältimine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Salvesta sait mallina käsk ei toetata ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri Avaldamisinfrastruktuur.


**Saidimalli ei saa luua või ei tööta õigesti**

- Mallis võib olla [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) puudu ja seda ei aktiveerita. Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa saidi loomiseks saidimalli kasutada.


- Kontrollige, et näha, kas loendid või teegid ületavad [loendivaate piirmäära piirmäära](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 üksused, kuna see võib blokeerida saidi malli loomine.


- Sait võib kasutada liiga palju ressursse ja seetõttu saidi Mall ületab 50 megabaidise (MB) piirang.


- On probleeme andmete kuvamisel loendist, mis kasutab Lookup veerg. Lisateabe saamiseks vaadake [malli loodud loend ei kuvata andmeid õige Lookup loendi SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Üksikasjalikuma teabe saamiseks levinud probleemide ja lahenduste kohta palun viidata, [luua ja kasutada saidimalle](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

