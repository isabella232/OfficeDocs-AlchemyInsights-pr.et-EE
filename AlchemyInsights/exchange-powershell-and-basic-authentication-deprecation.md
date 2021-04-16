---
title: Exchange PowerShell ja põhiautentimise kasutuselt eemaldamine
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813468"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell ja põhiautentimise kasutuselt eemaldamine

Uusimat teavet Exchange Online PowerShelliga ühenduse loomise kohta ilma põhiautentimiseta [vaadake siit](https://aka.ms/exops-docs). PowerShelli V2 moodul ei kasuta elementaarautentimist.

Pange tähele, et elementaarautentimine peab teie klientarvutis endiselt lubatud olema.
Uus PowerShelli V2 moodul kasutab modernautentimist, et luua ühendus kõigi REST-põhiste V2 cmdlet-käskude lubamiseks. Lisaks V2 cmdlet-käskudele pääsete juurde ka vanematele Remote PowerShelli (RPS) cmdlet-käskudele, mis nõuavad Remote PowerShelli seansi loomist. Windowsi masinal RPS-i seansi loomiseks on vajalik, et klientarvutis oleks WinRM põhiautentimine lubatud, isegi kui moodul kasutab teenuse autentimiseks modernautentimise mehhanismi. WinRM põhiautentimise konveierit kasutatakse modernautentimise tõendite transportimiseks. Kui klientarvutis on WinRM põhiautentimine keelatud, jätkavad V2 cmdlet-käsud töötamist (kuid vanemad RPS-i cmdlet-käsud mitte).
