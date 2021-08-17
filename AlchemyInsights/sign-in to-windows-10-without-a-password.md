---
title: Sisselogimine Windows 10 paroolita
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107504"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Sisselogimine Windows 10 paroolita

Selleks et vältida parooli tippimist Windows käivitamisel, soovitame kasutada ühte Windows Hello turvalisi sisselogimissuvandeid (nt PIN-kood, näotuvastus või sõrmejälg), kui see on saadaval. Kui soovite turvalise sisselogimise keelata, lugege allolevaid juhiseid "Logi sisse Windows 10".

**Turvaline Windows Hello alternatiivid konto paroolile**

Avage **Sätted > kontod > sisselogimissuvandid** (või klõpsake [siin).](ms-settings:signinoptions?activationSource=GetHelp) Kuvatakse saadaolevad sisselogimissuvandid. Näide.

![Sisselogimissuvandid.](media/sign-in-options.png)

Konfigureerimiseks klõpsake või puudutage ühte suvanditest. Järgmine kord, kui käivitate või Windows, saate parooli asemel kasutada uut suvandit. 

**Automaatne sisselogimine Windows 10**

**Märkus.** Automaatne sisselogimine on mugav, kuid see kehtestab turberiski, eriti juhul, kui teie arvutile pääsevad juurde mitu inimest. 

1. Klõpsake või **puudutage tegumiribal** nuppu Start.

2. Tippige **netplwiz** ja vajutage akna Kasutajakontod avamiseks sisestusklahvi (Enter).

3. Klõpsake **kasutajakontodes** kontot, kuhu soovite automaatselt sisse logida, kui Windows käivitub.

4. Tühjendage ruut "Kasutajad peavad selle arvuti kasutamiseks sisestama kasutajanime ja parooli".

    ![Kasutajad peavad sisestama kasutajanime ja parooli suvandi.](media/users-must-enter-username.png)

5. Klõpsake nuppu **OK**. Teil palutakse sisestada ja kinnitada valitud konto parool. Lõpetamiseks klõpsake nuppu **OK.** Kui Windows 10 käivitub, logitakse see automaatselt teie valitud kontole sisse.
