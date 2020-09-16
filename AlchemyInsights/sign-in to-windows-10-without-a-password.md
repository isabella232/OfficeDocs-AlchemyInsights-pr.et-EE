---
title: Windows 10 sisselogimine parooliga kasutamata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719949"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Windows 10 sisselogimine parooliga kasutamata

Et vältida parooli tippimist Windowsi käivitamisel, soovitame kasutada ühte Windows Hello turvalist sisselogimise suvandit (nt PIN-koodi, näo tuvastust või sõrmejälge), kui see on saadaval. Kui soovite kindlasti turvalise sisselogimise keelata, lugege allpool olevat jaotist "Automaatne sisselogimine opsüsteemi Windows 10".

**Turvaliste Windows Hello alternatiivid konto parooli**

Valige **sätted, > kontode > sisselogimise suvandid** (või klõpsake [siin](ms-settings:signinoptions?activationSource=GetHelp)). Saadaolevad sisselogimise suvandid on loetletud. Näiteks.

![Sisselogimise suvandid.](media/sign-in-options.png)

Selle konfigureerimiseks klõpsake või puudutage mõnda suvandit. Järgmine kord, kui käivitate või avate Windowsi, saate parooli asemel kasutada uut suvandit. 

**Windows 10 automaatne sisselogimine**

**Märkus**: Automaatne sisselogimine on otstarbekas, kuid see tutvustab turvariski, eriti juhul, kui teie arvuti on juurdepääsetav mitmele inimesele. 

1. Klõpsake või puudutage tegumiribal nuppu **Start** .

2. Tippige **netplwiz** ja vajutage akna Kasutajakontod avamiseks sisestusklahvi (ENTER).

3. Klõpsake jaotises **kasutajakontod**kontot, millele soovite Windowsi käivitumisel automaatselt sisse logida.

4. Tühjendage ruut "kasutajad peavad selle arvuti kasutamiseks sisestama kasutajanime ja parooli".

    ![Kasutajad peavad sisestama suvandi kasutajanimi ja parool.](media/users-must-enter-username.png)

5. Klõpsake nuppu **OK**. Teil palutakse valitud konto parool sisestada ja kinnitada. Lõpuleviimiseks klõpsake nuppu **OK** . Järgmine kord, kui Windows 10 käivitub, logib see automaatselt sisse teie valitud kontole.
