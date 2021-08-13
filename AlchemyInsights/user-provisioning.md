---
title: Kasutajate ettevalmistamine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971335"
---
# <a name="user-provisioning"></a>Kasutajate ettevalmistamine

- Kasutage nõudmisel [ettevalmistamise funktsiooni,](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) et kasutajat ette näha ja üksikasjalikke diagnostikafunktsioone tehtud toimingute kohta.
- Kasutajate ja rühmade ettevalmistamisega seotud probleemide tõrkeotsinguks lugege tõrkeotsingu juhendit [Kasutajad pole ette ettevalmistamise kohta.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Kui märkate, et kasutajad pole [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) ette ettevalmistamises, lugege teemat Azure Active Directory (AD) logide ettevalmistamine (eelvaade). Otsige kindla kasutaja logikirjeid.
- Käivitage ettevalmistamine regulaarselt uuesti, et püüda kinni kõik eelmises ettevalmistamise tsüklis vastamata jäänud kasutajad.
- Võimalik, et kasutajat/rühma pole ette ettevalmistamises, kuna meie teenusel pole veel olnud võimalust kasutajat hinnata. Vaadake üle juhised selle kohta, kui kaua ettevalmistamine aega võtab, ja edenemisriba ettevalmistamise konfiguratsioonilehel. Kui jaotises Täiendavad üksikasjad määratud püsiolekus on enne kuupäeva, mil kasutaja loodi/värskendati/kustutati, tähendab see, et me pole kasutajat veel hinnanud. Selle stsenaariumi korral on kõige parem oodata, kuni ettevalmistamise teenus lõpule jõuaks. Kui püsiolekut on saavutatud, soovitame Azure'i portaalis kasutajaliidese kaudu taaskäivitada.
  - Võtke arvesse, et meie teenus on teadlik ainult kasutaja/rühma muudatustest lähtesüsteemis (Azure Active Directory). Kui kasutaja/rühm eemaldatakse otse rakendusest (nt ServiceNow), ei tea me neid muudatusi ega pööra seda lähtesüsteemis oleva kasutaja oleku põhjal tagasi. Selle stsenaariumi korral on parem muudatus otse sihtrakenduses tagasi pöörata.
- Meie teenus hindas kasutajat/rühma ja määratles, et seda ei tohiks ette ettevalmistamise jaoks ette näha.
  - Kui olete määranud ulatuseks määratud kasutajad ja rühmad, kontrollige, kas kasutajale/rühmale on rakendus määratud.
  - Kui kasutajale/rühmale on määratud rakendus, veenduge, et neile ei määrata vaikejuurdepääsu rolli. Seda rolli ei saa kasutada ettevalmistamise jaoks.
  - Kui olete määranud atribuudipõhise ulatusefiltri, veenduge, et kasutaja vastaks teie määratud kriteeriumidele.
  - Kui kasutajad on sihtsüsteemis juba olemas ning lähte- ja sihtvaste kasutaja olek on juba olemas, ei võta me edasisi meetmeid.
- Meie teenus proovis kasutajat ette näha ja see nurjus. Nende stsenaariumide korral vaadake läbi ettevalmistamise logide vahekaart Tõrkeotsing ja soovitused.
  - Kasutaja nõutav atribuut võib olla puudu Azure Active Directory või ei vasta kolmanda osapoole rakenduse nõutavale vormingule. Näiteks võib kasutaja atribuudi Riik väärtuseks määrata Ameerika Ühendriigid, kui see peaks olema USA.
  - Atribuut on viitamisatribuut, mida sihtrakenduses veel pole. Viitamisatribuut on atribuut, mis osutab teisele objektile (nt rühma liikmele). Kasutaja ID oleks rühma liikmeatribuudis, kuid seda saab töödelda ainult siis, kui kasutajaobjekt, mille kohta see viitab, on juba olemas.
