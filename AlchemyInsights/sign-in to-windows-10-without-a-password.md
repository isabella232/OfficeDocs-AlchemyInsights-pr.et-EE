---
title: Sisselogimine Windows 10 parooli kasutamata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588277"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Sisselogimine Windows 10 parooli kasutamata

Et vältida parooli sisestamist Windowsi käivitamisel, soovitame kasutada ühte Windows Hello turvalise sisselogimise suvanditest, nagu PIN-kood, näotuvastus või sõrmejälg, kui see on saadaval. Kui soovite kindlasti turvalise sisselogimise keelata, lugege allolevaid juhiseid jaotisest "automaatselt sisse logida Windows 10".

**Secure Windows Hello alternatiivid konto parool**

Avage **sätted > kontod > Sisselogimissuvandid** (või klõpsake [siin](ms-settings:signinoptions?activationSource=GetHelp)). Saadaolevad Sisselogimissuvandid loetletakse. Näiteks.

![Sisselogimissuvandid.](media/sign-in-options.png)

Klõpsake või koputage selle konfigureerimiseks ühte suvandit. Järgmisel korral, kui käivitate või avate Windowsi, saate kasutada parooli asemel uut suvandit. 

**Sisselogimine automaatselt Windows 10-sse**

**Märkus**: Automaatne sisselogimine on mugav, kuid tutvustab turberiski, eriti kui teie arvutil on juurdepääs mitmele inimesele. 

1. Klõpsake või koputage tegumiribal nuppu **Start** .

2. Tippige **netplwiz** ja vajuta sisenema võti kasutajakontode akna avamiseks.

3. Klõpsake **kasutajakontode**kontol, kuhu soovite Windowsi käivitumisel automaatselt sisse logida.

4. Tühjendage märkeruut "kasutajad peavad sisestama kasutajanime ja parooli selle arvuti kasutamiseks".

    ![Kasutajad peavad sisestama kasutajanime ja parooli suvandi.](media/users-must-enter-username.png)

5. Klõpsake nuppu **OK**. Teil palutakse sisestada ja kinnitada valitud konto parool. Lõpetamiseks klõpsake nuppu **OK** . Järgmine kord, kui Windows 10 käivitub, läheb see automaatselt teie valitud kontole sisse.
