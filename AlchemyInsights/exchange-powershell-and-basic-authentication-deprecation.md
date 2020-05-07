---
title: Exchange PowerShell ja põhiautentimise kasutuselt eemaldamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015685"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell ja põhiautentimise kasutuselt eemaldamine

Uusimat teavet Exchange Online PowerShelliga ühenduse loomise kohta ilma põhiautentimiseta [vaadake siit](https://aka.ms/psbasicauth).

Pange tähele, et elementaarautentimine peab teie klientarvutis endiselt lubatud olema.
Uus PowerShelli V2 moodul kasutab modernautentimist, et luua ühendus kõigi REST-põhiste V2 cmdlet-käskude lubamiseks. Lisaks V2 cmdlet-käskudele pääsete juurde ka vanematele Remote PowerShelli (RPS) cmdlet-käskudele, mis nõuavad Remote PowerShelli seansi loomist. Windowsi masinal RPS-i seansi loomiseks on vajalik, et klientarvutis oleks WinRM põhiautentimine lubatud, isegi kui moodul kasutab teenuse autentimiseks modernautentimise mehhanismi. WinRM põhiautentimise konveierit kasutatakse modernautentimise tõendite transportimiseks. Kui klientarvutis on WinRM põhiautentimine keelatud, jätkavad V2 cmdlet-käsud töötamist (kuid vanemad RPS-i cmdlet-käsud mitte).
