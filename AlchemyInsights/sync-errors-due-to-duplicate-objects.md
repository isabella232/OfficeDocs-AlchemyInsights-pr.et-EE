---
title: 902 (vigade sünkroonimine dubleeritud objektide tõttu)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737337"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Vigade sünkroonimine dubleeritud objektide tõttu

Kui kataloogi sünkroonimine Microsoft 365 lõpeb, võidakse kuvada mõni järgmistest tõrketeadetest.

- Microsoft Online Services ei saa seda objekti värskendada, kuna selle objektiga seotud järgmistele atribuutidele on lisatud väärtused, mis võivad juba olla seotud mõne muu kohalikus kataloogis oleva objektiga.

- Teie Microsoft Online Services kataloogis on sama puhverserveri aadressiga sünkroonitud objekt juba olemas.

- Seda objekti ei saa värskendada, sest järgmised selle objektiga seostuvad atribuudid sisaldavad väärtusi, mis võivad juba olla seotud mõne muu kohaliku kataloogiteenuse objektiga: UserPrincipalName.

Probleemi tuvastamiseks ja lahendamiseks laadige alla ja käivitage [IdFix Dirsynci tõrke parandamise tööriist](https://www.microsoft.com/download/details.aspx?id=36832).

Lisateavet leiate teemast [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
