---
title: TeamViewer kasutamine Intune Devices kaugjuhtimiseks haldamiseks
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554973"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>TeamViewer kasutamine Intune Devices kaugjuhtimiseks haldamiseks

Intune ' i hallatavaid seadmeid saab [TeamViewer](https://www.teamviewer.com/)abil eemalt hallata.

Intune ' i haldamiseks funktsiooni TeamViewer abil tehke järgmist. 

Alustuseks Hankige mandaat alates TeamViewer, et häälestada TeamViewer konnektor Intune. See võimaldab administraatoril sisestada mandaate TeamViewer Connectori KASUTAJALIIDESE jaotises seadmed, ühekordne toiming, et luua link Intune ' i ja TeamViewer teenuse vahel.

**1. osa: seansi alustamine kaugarvutiga**

1. Valige jaotises **kõik seadmed**seade, millega soovite seansi alustada.
2. Alates **... **Valige **Uus Kaugabi seanss**.
3. Valige **Jah** , et kinnitada, et soovite luua seansi.
    Pärast seda, kui TeamViewer teenus on kinnitanud taotluse "uue serveri seansi alustamine", kuvatakse teile suvand **kaugabi käivitamiseks** seadme ülevaate (või Essentialsi) üksikasjade alusel. Paani laiendamiseks ja kaugabi oleku kuvamiseks valige Kuva **rohkem** .
4. Seansi alustamiseks administraatori poole valige **Käivita Kaugseanss** .
5. Valige TeamViewer binaarne (Windows) ja valige **Käivita**.<br/>
    **Märkus** Saate ignoreerida mis tahes veebibrauseri lehte, mis on avatud TeamViewer veebisaidile.

6. Kinnitage rakenduse TeamViewer taotlus teha muudatusi seadmes (ainult Windowsis).
7. TeamViewer rakendus käivitub ja sisaldab seansi koodi, et autentida ühendust kaugserveri seadmega.

**Osa 2: seadmes, mis on suunatud serveri seansile**

1. Avage Intune ettevõtte portaal.
2. Teatise lipu otsimine: "teie IT-administraator palub selle seadme juhtelementi Kaugabi seansi jaoks" ja valige teatis.
3. Valige TeamViewer rakenduse allalaadimine või TeamViewer rakenduse allalaadimine App Store ' ist ja valige **Käivita**.
    **Märkus** Saate ignoreerida mis tahes veebibrauseri lehte, mis on avatud TeamViewer veebisaidile.

4. Kinnitage rakenduse TeamViewer taotlus teha muudatusi seadmes (ainult Windowsis).
5. TeamViewer rakendus käivitub ja sisaldab seansi koodi, et autentida ühendust kaugserveri seadmega.
6. Hüpik küsib, kas soovite seansi avakuvale lubada.

**Märkus** TeamViewer teenus genereeritud seansi koodid on ainult ühekordseks kasutamiseks. Kui kaotate ühendust, peate tegema järgmist.

1. Sulgege TeamViewer rakenduse eksemplar kaugarvutis ja administraatori tööjaamas.
2. Sulgege Kaug-seadmes ettevõtte portaal.
3. Alustage administraatori portaalist uut uut kaugabi seanssi.
4. Uue teatise vastuvõtmiseks avage serveri seadmes uuesti ettevõtte portaal.
5. Laadige alla ja avage TeamViewer rakendus nii kaugarvutis kui ka administraatori tööjaamas.