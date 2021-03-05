---
title: Kasutaja ettevalmistamine
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481361"
---
# <a name="user-provisioning"></a>Kasutaja ettevalmistamine

- Kasuta [tellitavate ettevalmistuste](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) võimalusi kasutaja loomiseks ja üksikasjalike diagnostika tegemiseks võetud sammude kohta.
- Kasutajate ja rühmade ettevalmistamisel ilmneda võivate probleemide tõrkeotsing leiate teemast Tõrkeotsing [kasutajatele pole ette valmistatud](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Kui märkate, et kasutajaid pole ette valmistatud, lugege teemat [logide ettevalmistamine (eelvaade)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) Azure Active DIRECTORYS (ad). Saate otsida kindla kasutajaga seotud Logi kandeid.
- Värskendage aeg-ajalt ettevalmistusi, et püüda kõik kasutajad, kes on eelmises ettevalmistamise tsüklis vastamata.
- Kasutaja/rühm ei pruugi olla ette valmistatud, sest meie teenusel pole võimalust kasutajat veel hinnata. Vaadake juhiseid selle kohta, kuidas pikalt ette valmistada, ning ka edenemisriba lehel ettevalmistamine konfigureerimine. Kui jaotises täiendavad üksikasjad määratud püsiv olek on enne kasutaja loomise/värskendamise/kustutamise kuupäeva, tähendab see seda, et me pole kasutajat veel hinnanud. Selle stsenaariumi korral on parim asi, mida teha on oodata ettevalmistuste lõpuleviimiseks. Kui stabiilne olek on saavutatud, soovitame Azure ' i portaali KASUTAJALIIDESt uuesti käivitada.
  - Pange tähele, et meie teenus on ainult teadlikud kasutaja/rühma allikas süsteemis (Azure Active Directory). Kui kasutaja/rühm eemaldatakse otse rakendusest (nt ServiceNow), ei ole me nendest muudatustest teadlikud ja ei veereta seda tagasi, võttes aluseks lähteprogrammi kasutaja oleku. Selle stsenaariumi korral on soovitatav muudatus otse TARGETi rakenduses tagasi pöörata.
- Meie teenus hindas kasutajat/rühma ja see ei tohiks olla ette valmistatud.
  - Kui olete määranud kasutajatele ja rühmadele määratava ulatuse, siis kontrollige, kas rakendusele on määratud kasutaja/rühm.
  - Kui kasutajale/rühmale on määratud rakendus, veenduge, et need poleks määratud Accessi rollile. Seda rolli ei saa ettevalmistamisel kasutada.
  - Kui olete määranud atribuudi määramisel põhineva filtri, veenduge, et kasutaja vastab teie määratud kriteeriumidele.
  - Kui kasutajad on TARGETi süsteemis juba olemas ja kasutaja olek on allikas ja TARGETi vaste, ei võta me täiendavaid toiminguid.
- Meie teenus proovis kasutajat ette valmistada ja see ebaõnnestus. Nende stsenaariumide korral vaadake üle ettevalmistuste logide vahekaart tõrkeotsing ja soovitused.
  - Võimalik, et kasutaja nõutav atribuut on Azure Active Directorys puudu või ei vasta kolmanda osapoole rakenduse nõutud vormingule. Näiteks võib kasutaja atribuut Country määrata Ameerika Ühendriikidesse, kui see peaks olema meie.
  - Atribuut on viitamistervikluse, mis pole sihtrakenduse jaoks veel olemas. Viitamistervikluse on atribuut, mis viitab mõnele muule objektile (nt rühma liikmeks olevale kasutajale). Kasutaja ID oleks rühma atribuudi liige, kuid seda saab töödelda ainult siis, kui selle kasutaja objekt, millele see viitab, on juba olemas.
