---
title: 902 (duplikaatobjektide tõttu ilmnevad sünkroonimistõrked)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998786"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Duplikaatobjektide tõttu ilmnevad sünkroonimistõrked

Kui kataloogisünkroonimine lõpetatakse, võidakse kuvada üks järgmistest tõrketeadetest Microsoft 365.

- Seda objekti ei saa teenuses Microsoft Online Services värskendada, kuna selle objektiga seotud järgmistel atribuutidel on väärtused, mis võivad olla juba seostatud mõne muu objektiga teie kohalikus kataloogis.

- Sama puhverserveri aadressiga sünkroonitud objekt on teie Teenuse Microsoft Online Services kataloogis juba olemas.

- Seda objekti ei saa värskendada, kuna selle objektiga seotud järgmistel atribuutidel on väärtused, mis võivad juba olla seotud mõne muu objektiga teie kohalikes kataloogiteenustes: UserPrincipalName.

Probleemi tuvastamiseks ja lahendamiseks laadige alla ja käivitage [IdFix DirSynci tõrke parandamise tööriist.](https://github.com/Microsoft/idfix)

Lisateavet leiate teemast [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
