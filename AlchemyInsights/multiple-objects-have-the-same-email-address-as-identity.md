---
title: Mitmel objektil on sama meiliaadress identiteedina
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438931"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Mitmel objektil on sama meiliaadress identiteedina

**Mitu objekti**

Üks selle tõrke levinumatest põhjustest ei saa Outlook Web Accessi taotlust õigesti marsruutida, kui esineb mitu objekti, millel on sama meiliaadress identiteedina. Nende objektide leidmiseks käivitage järgmised käsud.

· Get-adressaat<email address>

· Get-User<email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact<email address>

· Hankimine-postkast <email address> – PublicFolder

· Hankimine-postkast <email address> – IncludeSoftDeletedMailbox

· Hankimine-postkast <email address> – InactiveMailboxOnly

Probleemi lahendamiseks eemaldage mitu sama e-posti identiteedi objekti ja veenduge, et kindla meili identiteediga on üks objekt ja selle adressaadi tüüp on UserMailbox.

**Sama aadressi kasutatakse nii ärikasutajate kui ka klientide postkastide jaoks**

Teine põhjus on see, kui sama aadressi kasutatakse nii ärikasutajate kui ka klientide postkastide jaoks. Sellisel juhul peab kasutaja muutma oma esmase tarbija pseudonüümi, kuni Cafe selle stsenaariumi toetab. See on püsiv viga, mis ei kao ilma sekkumiseta.

Lisateavet leiate teemast [Microsofti konto meiliaadressi või telefoninumbri muutmine](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).