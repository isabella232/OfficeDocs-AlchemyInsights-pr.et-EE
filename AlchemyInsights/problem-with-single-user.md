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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960147"
---
# <a name="problem-with-single-user"></a>Probleem ühe kasutajaga

- Võimalik, et kasutajat pole ette ettevalmistamises, kuna teenusel pole veel olnud võimalust kasutajat hinnata. Vaadake üle juhised selle kohta, kui kaua ettevalmistamine aega võtab, ja edenemisriba ettevalmistamise konfiguratsioonilehel. Kui jaotises Täiendavad üksikasjad määratud püsiolekus on enne kuupäeva, mil kasutaja loodi/värskendati/kustutati, tähendab see, et me pole kasutajat veel hinnanud. Selle stsenaariumi korral on kõige parem oodata, kuni ettevalmistamise teenus lõpule jõuaks.

  - Võtke arvesse, et meie teenus on teadlik ainult lähtesüsteemis (cloud HR) kasutaja tehtud muudatustest. Muudatuse tuvastamiseks ja Active Directorysse liikumiseks peab Azure AD lähtesüsteemis olema kehtiv muudatus.
- Ettevalmistamise teenus hindas kasutajat ja määratles, et seda ei tohiks ette ettevalmistamisele.
  - Kui olete määranud atribuudipõhise ulatusefiltri, veenduge, et kasutaja vastaks teie määratud kriteeriumidele.
  - Kui kasutajad on sihtsüsteemis juba olemas ning lähte- ja sihtvaste kasutaja olek on juba olemas, ei võta me edasisi meetmeid.
- Ettevalmistamise teenus proovis kasutajat ette näha ja see nurjus. Nende stsenaariumide korral vaadake läbi ettevalmistamise logide vahekaart Tõrkeotsing ja soovitused.
  - Kasutaja nõutav atribuut võib olla puudu asutusesiseses Active Directorys või Azure AD-s. Näiteks userPrincipalNamei või sAMAccountNamei põlvkonna reeglid ei genereeri õiget väärtust.
  - Vastendusatribuut (tavaliselt employeeId) ei lahenda kordumatut kasutajat asutusesiseses Active Directorys või Azure AD-s. Näiteks on AD-s kaks sama töötaja ID-ga kasutajat ja teenus tagastab tõrkekoodi, mis näitab sama lähtekirje duplikaatsihtkirjeid.

Ühe kasutaja ja rühmade logide läbivaatamiseks lugege teemat Konkreetse kasutajaga seotud probleemi ettevalmistamise [logide ülevaatamine.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
