---
title: Saidi või loendi salvestamine mallina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109200"
---
# <a name="save-site-or-list-as-a-template"></a>Saidi või loendi salvestamine mallina

SharePoint saidimallid on valmismääratlused, mis on mõeldud teatud ettevõtte vajadusele. Lisateavet leiate teemast [Mallide kasutamine erinevat tüüpi saitide SharePoint.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Siin on mõned levinumad probleemid või lahendused, mis on seotud saidi või loendi salvestamisega mallina SharePoint Veebiversioon.

**Nupp Salvesta saidi-/loendimall pole saadaval ega puudu.** 

- Malli funktsioonide lubamiseks peavad administraatorid lubama kohandatud skripti. Üksikasjalikud juhised leiate teemast Kohandatud skriptide [lubamine või keelamine.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Käsku Salvesta sait mallina ei toetata ja see võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri avaldamistaristut.


**Saidimalli ei saa luua või see ei tööta õigesti**

- Mall võib puududa [funktsioonist](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ja seda ei aktiveerita. Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa saidimalli abil saiti luua.


- Kontrollige, kas mõni loend või teek ületab [loendivaate](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) limiidi piirmäära 5000 üksust, kuna see võib blokeerida saidimalli loomise.


- Sait võib kasutada liiga palju ressursse ja seetõttu ületab saidimall 50 megabaidi (MB) piirangu.


- Otsinguveerge kasutava loendi andmete kuvamisel on probleeme. Lisateavet leiate teemast Malli genereeritud loend ei kuva SharePoint [Online'is õigest otsinguloendist pärit andmeid.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Lisateavet levinumate probleemide ja lahenduste kohta leiate teemast [Saidimallide loomine ja kasutamine.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

