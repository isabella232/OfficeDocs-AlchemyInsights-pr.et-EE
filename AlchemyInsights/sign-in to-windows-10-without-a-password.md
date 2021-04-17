---
title: Windows 10 sisselogimine ilma paroolita
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
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830542"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Windows 10 sisselogimine ilma paroolita

Windowsi käivitamisel parooli tippimise vältimiseks soovitame kasutada ühte Windows Hello turvalist sisselogimissuvandeid (nt PIN-kood, näotuvastus või sõrmejälg), kui see on saadaval. Kui soovite turvalise sisselogimise keelata, lugege allpool toodud juhiseid "Logi automaatselt windows 10 sisse".

**Secure Windows Hello alternatives to the account password**

Avage **Sätted > Kontod > sisselogimissuvandid** (või klõpsake [siin).](ms-settings:signinoptions?activationSource=GetHelp) Kuvatakse saadaolevad sisselogimissuvandid. Näide.

![Sisselogimissuvandid.](media/sign-in-options.png)

Konfigureerimiseks klõpsake või puudutage ühte suvanditest. Järgmine kord, kui käivitate või avate Windowsi, saate parooli asemel kasutada uut suvandit. 

**Windows 10 automaatne sisselogimine**

**Märkus.** Automaatne sisselogimine on mugav, kuid see kehtestab turberiski, eriti juhul, kui teie arvutile pääsevad juurde mitu inimest. 

1. Klõpsake või **puudutage tegumiribal** nuppu Start.

2. Tippige **netplwiz** ja vajutage akna Kasutajakontod avamiseks sisestusklahvi (Enter).

3. Klõpsake **kaustas Kasutajakontod** kontot, kuhu soovite Windowsi käivitamisel automaatselt sisse logida.

4. Tühjendage ruut "Kasutajad peavad selle arvuti kasutamiseks sisestama kasutajanime ja parooli".

    ![Kasutajad peavad sisestama kasutajanime ja parooli suvandi.](media/users-must-enter-username.png)

5. Klõpsake nuppu **OK**. Teil palutakse sisestada ja kinnitada valitud konto parool. Lõpetamiseks klõpsake nuppu **OK.** Järgmine kord, kui Windows 10 käivitub, logitakse see automaatselt teie valitud kontole sisse.
