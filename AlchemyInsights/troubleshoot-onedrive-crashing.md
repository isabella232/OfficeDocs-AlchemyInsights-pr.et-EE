---
title: OneDrive'i krahhide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748917"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive'i krahhide tõrkeotsing

Kui OneDrive jookseb korduvalt kokku, proovige järgmisi veaotsingu toiminguid.

**Veenduge, et registrivõtmeid pole seatud:**

1. Registriredaktori abil liikuge HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Kui DisableFileSyncNGSC on olemas ja seatud 1, avage võti ja muutke väärtuseks 0.
3. OneDrive'i käsitsi käivitamiseks avage menüü Start ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tippige otsinguväljale OneDrive ja seejärel klõpsake OneDrive'i töölauarakendust.

**OneDrive'i lähtestamine:**

Märkmed:

- OneDrive'i lähtestamine katkestab kõik olemasolevad sünkroonimisühendused (sh teie isikliku OneDrive'i, kui see on häälestatud).
- OneDrive'i arvutist lähtestamisel faile ega andmeid ei kaotata.

**OneDrive'i lähtestamiseks**

1. Avab dialoogi Käivita, vajutades Windowsi klahvi ja r.
2. Tippige %localappdata%\Microsoft\OneDrive\onedrive.exe /reset ja vajutage nuppu OK. Käsuaken võidakse kuvada korraks.
3. OneDrive'i käsitsi käivitamiseks avage menüü Start ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tippige otsinguväljale OneDrive ja seejärel klõpsake OneDrive'i töölauarakendust.

Märkmed:

- Kui olete enne lähtestamist otsustanud sünkroonida ainult mõned kaustad, peate seda uuesti tegema, kui sünkroonimine on lõpule viidud. Lisateabe [saamiseks lugege lisateavet jaotisest Valige, millised OneDrive'i kaustad arvutiga sünkroonida.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  
- Peate selle oma isikliku OneDrive'i ja OneDrive for Businessi jaoks lõpule viima.