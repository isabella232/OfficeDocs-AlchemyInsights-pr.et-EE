---
title: 902 (sünkroonimise tõrgete tõttu dubleeritud objektid)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420870"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sünkroonimise tõrgete tõttu dubleeritud objektid

Võite saada ühe järgmistest kataloogi sünkroonimise lõppemisel:

- Ei saa värskendada selle objekti Microsoft Online Services, sest järgmise seotud objekt on väärtused, mida juba võib olla seotud mõne muu objekti oma kohaliku kataloogis.

- Microsofti võrguteenuste kataloogi sünkroonitud objekti koos sama meiliaadress on juba olemas.

- Ei saa värskendada selle objekti, sest järgmised atribuudid, mis on seostatud selle objekti on väärtused, mis võib juba olla seotud teise objekti kohalik directory Services: UserPrincipalName.

Tuvastada ja lahendada see probleem, alla laadida ja [IdFix DirSync vea parandamise tööriist](https://www.microsoft.com/download/details.aspx?id=36832).

Lisateabe saamiseks vt [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
