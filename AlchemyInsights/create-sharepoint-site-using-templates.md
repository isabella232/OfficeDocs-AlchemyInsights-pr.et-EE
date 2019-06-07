---
title: Luua saidi SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753704"
---
# <a name="create-sharepoint-sites-using-templates"></a>Luua SharePointi saitide abil

SharePointi saidi templates on mõeldud ärivaldkonnas vaja umbes Varemkoostatud mõisted. Lisateabe saamiseks vt [kasutamine malle luua erinevat tüüpi SharePointi saitidele](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Siin on mõned ühised probleemid/lahendusi seoses salvestamine on saidi- või mallina Sharepoint Online. 

**Salvesta saidilt/sellest loendist malli nupp ei ole saadaval või puudub**

Administraatorid tuleb lubada kohandatud skripti malli funktsioonide lubamiseks. Üksikasjalikud näited ja kaalutluste kohta leiate 

- [Või mitte kohandatud skripti](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Salvesta saidi malli käsku ei toetata ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri Publishing infrastruktuuri.

Saidimalli ei saa luua või ei tööta õigesti.

Malli võib puududa [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ja ei Aktiveeri. Kui funktsioon ei ole saadaval praeguses saidikogumis aktiveerida, ei saa saidimalli abil saidi loomine.

- Kontrollige, kui loendeid ja teeke ületab [Loendivaateläve piir](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 üksust, kuna see võib takistada saidi malli loomine.

- Sait kasutab liiga palju ressursse ja seega saidi malli ületab 50 MB.


- On probleeme, mis kasutab otsinguveeru andmed kuvatud. Lisateabe saamiseks vt [mall loodud loendis ei kuvata SharePoint Online õige otsinguloendis andmeid](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Täpsemat infot üldlevinud probleeme ja lahendusi, Palun kontrollige [saidimallide loomine ja kasutamine](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



