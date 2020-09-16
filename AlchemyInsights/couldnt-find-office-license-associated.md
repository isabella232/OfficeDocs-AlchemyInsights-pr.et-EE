---
title: Microsoft 365 rakenduste parandamine ei leia Office ' i litsentsidega seostuvat sõnumit
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747691"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Microsoft 365 rakenduste parandamine "ei saanud Office ' i litsentsidega seostuvat teadet"

Kui teile kuvatakse see teade, proovige teha järgmist.

1. Kontrollige oma tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Vaadake teemat [Microsoft 365 URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Eemaldage mõjutatud kasutaja [Office ' i litsents ja määrake see](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) uuesti. 
3. Avage Office ' i rakendus ja [logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevast kasutajakontost.
4. Avage Windowsi sätted > **kontode**  >  **Meilikontod & kontod**ja eemaldage kõik töökontod, v. a mõjutatud konto.
5. Avage Windowsi sätted > **kontode**  >  **juurdepääs tööle või koolile**ning kõigi Töökontode, v. a mõjutatud kontoga ühenduse katkestamine.
6. Lähtestage Office ' i aktiveerimise olek. [Vaadake, kuidas](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logige](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sisse mõjutatud kasutaja kontoga.

Täiendavate lahenduste leidmiseks lugege artiklit [Office ' i litsentsimata toodete ja aktiveerimise tõrgete](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)tõrkeotsing.