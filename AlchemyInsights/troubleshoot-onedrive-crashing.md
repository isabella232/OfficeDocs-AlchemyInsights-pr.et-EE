---
title: OneDrive'i krahhide tõrkeotsing
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826195"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive'i krahhide tõrkeotsing

Kui OneDrive jookseb korduvalt kokku, proovige järgmisi tõrkeotsingutoiminguid.

**Veenduge, et registrivõtmed poleks määratud.**

1. Liikuge registriredaktori abil HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Kui DisableFileSyncNGSC on olemas ja selle väärtuseks on seatud 1, avage klahv ja muutke väärtus väärtuseks 0.
3. OneDrive'i käsitsi käivitamiseks valige Start ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tippige otsinguväljale OneDrive ja seejärel klõpsake OneDrive'i töölauarakendust.

**OneDrive'i lähtestamine.**

Märkmed:

- OneDrive'i lähtestamisel katkestatakse kõik olemasolevad sünkroonimisühendused (sh teie isiklik OneDrive, kui see on häälestatud).
- Te ei kaota faile ega andmeid, kui lähtestate OneDrive'i oma arvutis.

**OneDrive'i lähtestamiseks tehke ühte järgmistest.**

1. Dialoogiboksi Käivita avamiseks vajutage klahvikombinatsiooni Windowsi klahv ja R.
2. Tippige %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja vajutage nuppu OK. Käsuaken võidakse kuvada lühidalt.
3. OneDrive'i käsitsi käivitamiseks valige Start ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tippige otsinguväljale OneDrive ja seejärel klõpsake OneDrive'i töölauarakendust.

Märkmed:

- Kui otsustasite enne lähtestamist sünkroonida ainult mõned kaustad, peate seda uuesti tegema, kui sünkroonimine on lõpule viidud. Lisateavet [leiate teemast Valige, milliseid OneDrive'i kaustu arvutiga](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   sünkroonida.
- Peate selle lõpule viima isikliku OneDrive'i ja OneDrive for Businessi jaoks.