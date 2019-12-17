---
title: SharePoint Online ' i saidi loomine
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052465"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePointi saitide loomine mallide abil

SharePointi saidimallid on eelehitatud määratlused, mis on mõeldud konkreetse ärivajaduse ümber. Lisateavet leiate jaotisest [mallide kasutamine erinevat tüüpi SharePointi saitide loomiseks](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Siin on mõned levinud probleemid/lahendused saidi või loendi salvestamisel mallina SharePoint Online ' is. 

**Saidi/loendimalli nupu salvestamine pole saadaval või puudub**

Administraatorid peavad lubama kohandatud skripti malli funktsioonide lubamiseks. Üksikasjalikke samme, näiteid ja kaalutlusi vt 

- [Kohandatud skripti lubamine või vältimine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Salvesta sait mallina käsk ei toetata ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri Avaldamisinfrastruktuur.

**Saidimalli ei saa luua või ei tööta õigesti**

Mallis võib olla [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) puudu ja seda ei aktiveerita. Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa saidi loomiseks saidimalli kasutada.

- Kontrollige, et näha, kas loendid või teegid ületavad [loendivaate piirmäära piirmäära](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 üksused, kuna see võib blokeerida saidi malli loomine.

- Sait võib kasutada liiga palju ressursse ja seetõttu saidi Mall ületab 50 MB piirangu.


- On probleeme andmete kuvamisel loendist, mis kasutab Lookup veerg. Lisateabe saamiseks vaadake [malli loodud loend ei kuvata andmeid õige Lookup loendi SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Üksikasjalikuma teabe saamiseks levinud probleemide ja lahenduste kohta kontrollige palun [Loo ja kasuta saidimalle](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



