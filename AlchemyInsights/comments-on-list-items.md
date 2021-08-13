---
title: Kommentaarid loendiüksuste kohta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995474"
---
# <a name="comments-on-list-items"></a>Kommentaarid loendiüksuste kohta

Kasutajad saavad vaadata kõiki loendiüksuse kommentaare ja filtreerida vaadete vahel, kus kuvatakse üksusega seotud kommentaarid või tegevused.

Enne kommentaaride lisamiseks ja kustutamiseks peavad kasutajad teadma järgmist.

- Kommentaarid järgivad õiguste sätteid, mis on SharePoint.
- Klassikalistes loendites, mis pole veel valmis, et neid kuvada kaasaegsetes kasutajaliidestes (nt ülesandeloendites), pole seda kommentaarifunktsiooni.
- Selle väljaandega pole Teams loendite kommenteerimine saadaval.
- Otsing ei indekseeri kommentaare.

Administraatorid saavad selle funktsiooni organisatsiooni tasemel keelata, muutes **cmdlet-käsu Set-SPOTenant** PowerShell parameetrit **CommentsOnListItemsDisabled.**

Praegu ei saa saidil või loenditasemel kommenteerimist keelata. Loodame, et need juhtelemendid on hilisemas värskenduses, tõenäoliselt 2021. aasta esimeses kvartalis.
