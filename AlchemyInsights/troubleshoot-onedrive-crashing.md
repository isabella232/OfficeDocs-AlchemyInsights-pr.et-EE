---
title: Krahhide OneDrive tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921003"
---
# <a name="troubleshoot-onedrive-crashes"></a>Krahhide OneDrive tõrkeotsing

Kui OneDrive jookseb korduvalt kokku, proovige järgmisi tõrkeotsingutoiminguid.

**Veenduge, et registrivõtmed poleks määratud.**

1. Liikuge registriredaktori abil HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Kui DisableFileSyncNGSC on olemas ja selle väärtuseks on seatud 1, avage klahv ja muutke väärtus väärtuseks 0.
3. Käivitage OneDrive käsitsi, avakuvale ![Vajutage Windows klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tippige OneDrive otsinguväljale tekst ja seejärel klõpsake OneDrive töölauarakendust.

**Lähtesta OneDrive.**

Märkmed:

- Lähtestamine OneDrive katkestab kõik olemasolevad sünkroonimisühendused (sh teie isiklikud ühendused OneDrive kui see on häälestatud).
- Kui lähtestate oma arvutis OneDrive, ei kaota te faile ega andmeid.

**Lähtestamiseks OneDrive.**

1. Dialoogiboksi Käivita avamiseks vajutage klahvikombinatsiooni Windows R.
2. Tippige %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja vajutage nuppu OK. Käsuaken võidakse kuvada lühidalt.
3. Käivitage OneDrive käsitsi, avakuvale ![Vajutage Windows klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tippige OneDrive otsinguväljale tekst ja seejärel klõpsake OneDrive töölauarakendust.

Märkmed:

- Kui otsustasite enne lähtestamist sünkroonida ainult mõned kaustad, peate seda uuesti tegema, kui sünkroonimine on lõpule viidud. Lisateavet [leiate teemast OneDrive, milliseid kaustu arvutiga](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   sünkroonida.
- Peate selle lõpule viima oma isiklike OneDrive ja OneDrive for Business.