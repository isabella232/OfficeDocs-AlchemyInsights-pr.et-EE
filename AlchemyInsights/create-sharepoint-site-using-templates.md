---
title: Saidi loomine SharePoint Online ' is
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732215"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePointi saitide loomine mallide abil

Saidi salvestamine mallina pole toetatud moodsa suhtluse või meeskonnatöö saitidega. Lisateavet mallide kasutamise kohta leiate teemast [SharePointi saidi salvestamine, allalaadimine ja üleslaadimine mallina](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Siin on mõned levinud probleemid/lahendused seoses saidi või loendi salvestamisega mallina SharePoint Online ' is. 

**Nupp Salvesta saidi/loendi Mall pole saadaval või puudub**

Administraatorid peavad lubama kohandatud skripti malli funktsioonide lubamiseks. Üksikasjalikud juhised leiate teemast näited ja kaalutlused 

- [Kohandatud skripti lubamine või keelamine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Käsk Salvesta sait mallina pole toetatud ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri avaldamise infrastruktuuri.

**Saidimalli ei saa luua või see ei tööta õigesti**

Mallil võib olla [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) puudu ja see ei aktiveeru. Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa te saiti saidi loomiseks kasutada.

- Saate vaadata, kas loendid või teegid ületavad 5000 üksuste [loendivaate](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) piirmäära, kuna see võib saidi malli loomist blokeerida.

- Sait võib kasutada liiga palju ressursse ja seetõttu ületab saidimall 50 MB piiri.


- On probleeme, mis kuvavad andmeid otsinguveeru kasutavast loendist. Lisateavet leiate teemast [mallide põhjal loodud loend ei kuva SharePoint Online ' is õigete otsinguväljade andmeid](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Üksikasjalikumat teavet levinud probleemide ja lahenduste kohta leiate teemast [saidimallide loomine ja kasutamine](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



