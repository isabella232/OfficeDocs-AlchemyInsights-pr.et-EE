---
title: Teenuse osutamise teenuse konfigureerimine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481853"
---
# <a name="configuring-the-provision-service"></a>Teenuse osutamise teenuse konfigureerimine

Kui soovite, et automatiseeritud kasutaja ettevalmistamine töötaks, on Azure AD-s vaja kehtivaid mandaate, mis võimaldavad tal luua ühenduse tööpäevaga veebiteenuste API Lisaks kinnitatakse, et kui kasutaja saab luua ühenduse AD-domeeniga seotud Azure AD Connecti agendiga, siis kinnitab see, et tööpäeval töötav nupp Test Connection to AD Useri ettevalmistamine.

Kui Azure ' i portaalis kuvatakse mandaadi salvestamisel tõrge, järgige allpool soovitatud juhiseid.

1. Veenduge, et olete konfigureerinud tööpäevade integreerimise süsteemi kasutajakonto, nagu on näidatud jaotises õpetus, et [konfigureerida integratsiooni süsteemi kasutaja tööpäevas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Veenduge, et Azure AD Connecti ettevalmistamine agendi teenus töötab ja töötab teie kohapealses Windowsi serveris teenuste halduskonsooli abil. Samuti saate kontrollida agendi olekut Azure ' i portaalis, klõpsates nuppu Kuva kohapealsed agendid.
3. Veenduge, et sisestate välja "tööpäevade username" väärtuse, kasutades vormingut username@workday-rentniku nimi. Kui tööpäev – rentniku nimi on puudu, siis tööpäevade autentimine nurjub.
4. Kui konfigureerite integratsiooni tööpäevade rakendamise rentniku jaoks, arvestage oma tööpäevade rentniku ajastatud seisakute tundi. Tööpäeval on planeeritud aeg selle rakendamiseks rentnike jaoks nädalavahetustel (tavaliselt reede õhtul kuni laupäeva hommikul) ja Ühenduvus ebaõnnestumised selle seisakute aknas on teadaolev probleem, mis automaatselt lahendatakse kohe, kui rakendamise rentnikud on tagasi võrgus.
5. Harvadel juhtudel võite seda viga näha ka juhul, kui selle integreerimise süsteemi kasutaja parool on rentniku värskendamise tõttu muudetud või kui konto on lukustatud või aegunud olekus. Palun kontrolli oma tööpäevade administraatoriga integreerimise süsteemi kasutaja olekut.

Lisateavet tööpäevade automaatseks ettevalmistamiseks konfigureerimise kohta leiate teemast [õpetus: tööpäevade automaatseks](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)ettevalmistamiseks konfigureerimine.
