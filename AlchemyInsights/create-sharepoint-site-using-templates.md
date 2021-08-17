---
title: Saidi loomine SharePoint Online'is
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057962"
---
# <a name="create-sharepoint-sites-using-templates"></a>Mallide SharePoint saitide loomine

Kaasaegsed suhtlus- ja meeskonnatöö saidid ei toeta saidi mallina salvestamise võimalust. Mallide kasutamise kohta leiate lisateavet teemast [SharePointi saidi salvestamine, allalaadimine ja üleslaadimine mallina](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Siin on mõned levinumad probleemid/lahendused sharepoint Online'is saidi või loendi mallina salvestamisel. 

**Saidi-/loendimalli salvestamise nupp pole saadaval või puudub**

Malli funktsioonide lubamiseks peavad administraatorid lubama kohandatud skripti. Üksikasjalikud juhised, näited ja kaalutlused leiate teemast 

- [Kohandatud skripti lubamine või keelamine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Käsku Salvesta sait mallina ei toetata ja see võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri avaldamistaristut.

**Saidimalli ei saa luua või see ei tööta õigesti**

Mall võib puududa [funktsioonist](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ja seda ei aktiveerita. Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa saidimalli abil saiti luua.

- Kontrollige, kas mõni loend või teek ületab [loendivaate](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) limiidi piirmäära 5000 üksust, kuna see võib blokeerida saidimalli loomise.

- Sait võib kasutada liiga palju ressursse ja seetõttu ületab saidimall 50 MB piirangu.


- Otsinguveerge kasutava loendi andmete kuvamisel on probleeme. Lisateavet leiate teemast Malli genereeritud loend ei kuva SharePoint [Online'is õigest otsinguloendist pärit andmeid.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Levinumate probleemide ja lahenduste kohta leiate lisateavet teemast [Saidimallide loomine ja kasutamine.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



