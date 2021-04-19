---
title: Teamsi sisselogimistõrge AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821983"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Teamsi sisselogimistõrge AADSTS9000411

Microsoft Teamsi sisselogimisel võidakse kuvada tõrketeade: Kahjuks on meil probleeme **AADSTS9000411i sisselogimisega: taotlus pole õigesti vormindatud. Parameeter "login_hint" on dubleeritud.**

Selle probleemi lahendamiseks veenduge, et teie Microsoft Teamsi kliente värskendatakse. Lisateavet kliendi värskendamise kohta leiate teemast [Microsoft Teamsi värskendamine.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Kui te ei saa mingil põhjusel klientrakendust värskendada, tühjendab klientrakendusest väljalogimine enamik vahemällu talletatud andmeid. Kui teil on pärast sisselogimist endiselt probleeme, sulgege Teams ja tühjendage oma kliendi vahemälu, tehes järgmist.
1. Sulgege Microsoft Teams.
2. Avage: %appdata%\microsoft\teams ja kustutage kõik failid.
3. Avage Microsoft Teams uuesti.
