---
title: Kirjutuskaitstud hoolduse sõnumi katsel kasutada SharePointi või OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051277"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Kirjutuskaitstud hoolduse sõnumi katsel kasutada SharePointi või OneDrive

Kasutajad võivad saada **kirjutuskaitstud hoolduse** sõnumi katsel kasutada SharePointi või OneDrive üks järgmistest tingimustest. 

-   Planeeritud või aktiivne hooldustegevus.  Kontrollige neid, liikudes [sõnumikeskuse](https://portal.office.com/adminportal/home#/messagecenter)juurde.
-   Kõrge prioriteediga aktiivne teenindusjuhtum, mis võib tekkida. Kontrollige kõik nõud/intsidendid navigeerides [teenuse tervis](https://portal.office.com/adminportal/home#/servicehealth).
-   Väike auto-tervendav taastamise stsenaarium, mis võib juhtuda ootamatu sündmuste serverid, mis võivad kesta vähem kui 30 min või nii. 
    
    Nende väiksemate tagasimaksete jaoks pole sõnumikeskust ega teenuse Health postitusi, kuid peaksite varsti tagasi normaalseks.

Väga vähe kordi me täheldas, et üks eespool loetletud kolmest stsenaariumit on põhjus ja teenus on taastatud, kuid kasutajate brauseri vahemälu ei ole lahendatud.

Palun proovige tühjendada brauseri vahemälu enne navigeerimist saidile.

1. Valige oma Microsoft Edge ' i brauseris **sätted**ja seejärel **Privaatsus ja turve**.
2. Valige jaotises **Tühjenda sirvimine**käsk **Vali, mida tühjendada**.
3. Valige **küpsised ja salvestatud veebisaidi andmed**ning valige **Tühjenda**.

>[!Note] 
> Need sammud võivad erineda, kui kasutate muid brausereid nagu Mozilla Firefox või Google Chrome.

>[!Note] 
> Teine võimalus oleks avada SharePointi saidi või OneDrive uues InPrivate-aknas.