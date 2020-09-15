---
title: 'Tõrge: selle arvuti reeglid ei ühti'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690959"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Tõrge: selle arvuti reeglid ei ühti

Selle teadaoleva probleemi värskendatud oleku vaatamiseks lugege selle [arvuti reegleid, mis ei vasta Microsoft Exchange ' i reeglitele.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlooki meeskond on rakendanud lahenduse järgus 12928,10000. Fix on juba Insider Fast ja läheb igakuise kanali juuni lõpus 2020. Kui teil on püsiv järk, võite saada viiba "milliseid reegleid soovite säilitada" viimast korda. Valige küsimisel server ja seejärel naaske Outlookis ja lubage kõik keelatud reeglid uuesti.

Kui lahendus on saadaval, kasutage järgmist lahendust.

**Lahendus**: Viimatised aruanded on ilmnenud nende jaoks, kes on Outlooki töölaual loonud ainult klientrakenduste reegleid. Kui jätkate probleemi, kaaluge reeglite kustutamist ja seejärel looge ja redigeerige reegleid ainult OWA-s (Outlook Web App), kuni probleem laheneb.

Kui te ei saa reegleid käsitsi kustutada, saate Outlooki käsu käivitada Outlooki käivitamisel, käivitades Outlook.exe/Cleanrules. See toiming kustutab nii kliendi kui ka serveri reeglid. See kustutab kõik Outlooki profiilis olevate kontode reeglid. See käsk on täiendavalt dokumenteeritud käsurea lülitite artiklis.

