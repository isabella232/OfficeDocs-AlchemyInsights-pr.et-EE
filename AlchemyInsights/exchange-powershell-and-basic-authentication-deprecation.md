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
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069240"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell ja põhiautentimise kasutuselt eemaldamine

Uusimat teavet Exchange Online PowerShelliga ühenduse loomise kohta ilma põhiautentimiseta [vaadake siit](https://aka.ms/exops-docs). PowerShelli V2 moodul ei kasuta elementaarautentimist.

Pange tähele, et elementaarautentimine peab teie klientarvutis endiselt lubatud olema.
Uus PowerShelli V2 moodul kasutab modernautentimist, et luua ühendus kõigi REST-põhiste V2 cmdlet-käskude lubamiseks. Lisaks V2 cmdlet-käskudele pääsete juurde ka vanematele Remote PowerShelli (RPS) cmdlet-käskudele, mis nõuavad Remote PowerShelli seansi loomist. Windowsi masinal RPS-i seansi loomiseks on vajalik, et klientarvutis oleks WinRM põhiautentimine lubatud, isegi kui moodul kasutab teenuse autentimiseks modernautentimise mehhanismi. WinRM põhiautentimise konveierit kasutatakse modernautentimise tõendite transportimiseks. Kui klientarvutis on WinRM põhiautentimine keelatud, jätkavad V2 cmdlet-käsud töötamist (kuid vanemad RPS-i cmdlet-käsud mitte).
