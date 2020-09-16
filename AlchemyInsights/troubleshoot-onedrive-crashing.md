---
title: OneDrive ' i tõrkeotsing jookseb kokku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664994"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive ' i tõrkeotsing jookseb kokku

Kui OneDrive jookseb korduvalt kokku, proovige järgmisi veaotsingu toiminguid.

**Veenduge, et registrivõtmed pole määratud.**

1. Registriredaktori abil Navigeerige HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Kui DisableFileSyncNGSC on olemas ja see on seatud väärtusele 1, avage võti ja muutke väärtust väärtuseks 0.
3. OneDrive ' i käsitsi käivitamine, minnes avakuvale ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tippige otsinguväljale sõna OneDrive ja seejärel klõpsake OneDrive ' i töölauarakenduse nuppu.

**OneDrive ' i lähtestamine.**

Märkmete

- OneDrive ' i lähtestamisel lahutatakse kõik teie olemasolevad sünkroonimise ühendused (sh teie isiklik OneDrive, kui olete häälestanud).
- Te ei kaota faile ega andmeid, kui lähtestate OneDrive ' i oma arvutis.

**OneDrive ' i lähtestamiseks tehke järgmist.**

1. Dialoogiboksi Käivita avamiseks vajutage klahvikombinatsiooni Windowsi klahv ja R.
2. Tippige% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset ja vajutage nuppu OK. Käsuviiba aken võib olla lühike.
3. OneDrive ' i käsitsi käivitamine, minnes avakuvale ![Vajutage Windowsi klahvi](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tippige otsinguväljale sõna OneDrive ja seejärel klõpsake OneDrive ' i töölauarakenduse nuppu.

Märkmete

- Kui olete enne lähtestamist valinud vaid mõne kausta sünkroonimise, peate seda uuesti tegema, kui sünkroonimine on lõpule viidud. Lisateavet leiate teemast [OneDrive ' i kaustade valimine arvutiga sünkroonimiseks](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- Peate selle täitma oma isikliku OneDrive ' i ja OneDrive for Businessi jaoks.