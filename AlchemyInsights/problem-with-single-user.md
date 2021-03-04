---
title: Probleem ühe kasutajaga
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
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429711"
---
# <a name="problem-with-single-user"></a>Probleem ühe kasutajaga

- Kasutaja ei pruugi olla ette valmistatud, sest teenusel pole olnud võimalust kasutajat veel hinnata. Vaadake juhiseid selle kohta, kuidas pikalt ette valmistada, ning ka edenemisriba lehel ettevalmistamine konfigureerimine. Kui jaotises täiendavad üksikasjad määratud püsiv olek on enne kasutaja loomise/värskendamise/kustutamise kuupäeva, tähendab see seda, et me pole kasutajat veel hinnanud. Selle stsenaariumi korral on parim asi, mida teha on oodata ettevalmistuste lõpuleviimiseks.

  - Pange tähele, et meie teenus on teadlik ainult lähteprogrammi kasutaja muudatustest (pilveteenuse HR). Azure AD allikas süsteemis peab olema kehtiv muudatus, mis tuvastab muudatuse ja kasutab seda Active Directorys.
- Ettevalmistamise teenus hindas kasutajat ja see ei tohiks olla ette valmistatud.
  - Kui olete määranud atribuudi määramisel põhineva filtri, veenduge, et kasutaja vastab teie määratud kriteeriumidele.
  - Kui kasutajad on TARGETi süsteemis juba olemas ja kasutaja olek on allikas ja TARGETi vaste, ei võta me täiendavaid toiminguid.
- Teenuse ettevalmistamine proovis kasutajat ette valmistada ja see ebaõnnestus. Nende stsenaariumide korral vaadake üle ettevalmistuste logide vahekaart tõrkeotsing ja soovitused.
  - Kasutaja nõutav atribuut võib puududa kohapealsest Active Directory või Azure AD-s. Näiteks userPrincipalName või sAMAccountName loomise reeglid ei teeni õiget väärtust.
  - Vastavat atribuuti (tavaliselt employeeId) ei lahendata kohapealse Active Directory või Azure AD ainulaadse kasutajana. Näiteks on kaks kasutajat, kellel on sama employeeId AD ja teenus annab tõrketeate, mis viitab sama Allikatähise kahekordsetele kirjetele.

Kui soovite vaadata ühe kasutaja ja rühma logisid, lugege teemat [konkreetse kasutajaga seotud probleemi paranduste läbivaatus](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
