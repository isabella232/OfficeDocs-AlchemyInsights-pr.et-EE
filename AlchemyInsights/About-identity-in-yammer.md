---
title: Teave identiteedi kohta Yammeris
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148235"
---
# <a name="about-identity-in-yammer"></a>Teave identiteedi kohta Yammeris

Identiteediga seotud probleemide vältimiseks on soovitatav, et kõik võrgud võtaksid järgmist.

1. Jõustada Office 365 identiteedi pärast ettevalmistamine Microsoft 365 kontode kasutajatele Azure AD veendumaks, et kõik kasutajad sisse logida, kasutades oma esmane Microsoft 365 konto. Lisateavet leiate teemast [Office 365 identiteedi jõustamine Yammeri kasutajate jaoks](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolideerige mitu Yammeri võrku. Pärand Yammeri konfiguratsioonid võimaldavad mitme Yammeri võrgu ühe rentnikuga ühendada. Lisateavet leiate teemast [Võrgu migreerimine – mitme Yammeri võrgu konsolideerimine](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Soovi korral jõustage Yammeri litsentsimine, et blokeerida kasutajad Yammerist, kui neil pole litsentsi. Lisateavet leiate teemast [Yammeri kasutajalitsentside haldamine teenusekomplektis Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Lõpuks auditeerida kasutajate loend vanemate Yammeri võrkude ja peatada pärand kasutajad. Soovitatav on kasutajad kustutamise asemel peatada (desaktiveerida) kuna kustutamine on pöördumatu. Lisateavet leiate teemast [Yammeri kasutajate auditeerimine teenusekomplektiga Office 365 ühendatud võrkudes](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) ja [Kasutajate eemaldamine](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Yammeri konfigureerimisel nende juhiste abil saate konfigureerida ka oma Yammeri võrgu Microsoft 365 native mode jaoks. Lisateavet leiate teemast [Yammeri võrgu konfigureerimine Microsoft 365 native mode jaoks](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).