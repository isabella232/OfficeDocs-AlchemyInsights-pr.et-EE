---
title: 902 (sünkroonimise tõrgete tõttu dubleeritud objektid)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757991"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sünkroonimise tõrgete tõttu dubleeritud objektid

Võite saada ühe järgmistest kataloogi sünkroonimise lõppemisel:

- Ei saa värskendada selle objekti Microsoft Online Services, sest järgmise seotud objekt on väärtused, mida juba võib olla seotud mõne muu objekti oma kohaliku kataloogis.

- Microsofti võrguteenuste kataloogi sünkroonitud objekti koos sama meiliaadress on juba olemas.

- Ei saa värskendada selle objekti, sest järgmised atribuudid, mis on seostatud selle objekti on väärtused, mis võib juba olla seotud teise objekti kohalik directory Services: UserPrincipalName.

Tuvastada ja lahendada see probleem, alla laadida ja [IdFix DirSync vea parandamise tööriist](https://www.microsoft.com/download/details.aspx?id=36832).

Lisateabe saamiseks vt [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
