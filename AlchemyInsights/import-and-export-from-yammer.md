---
title: Yammeri importimine ja eksportimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035438"
---
# <a name="import-and-export-from-yammer"></a>Yammeri importimine ja eksportimine

**Importimine**

Kasutaja – impordi suvandid sõltuvad sellest, kas teie Yammeri võrk on [Microsoft 365 jaoks kohalik režiim](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)või mitte.

- **Muu režiim**: kasutajaid saab importida rühmadesse, kasutades [Lisa aadressiraamatust](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (Limit to 100 kasutajad) rühma sätetes või võrgu kaudu, mis kasutab [hulgi värskendust](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) võrgu administraatorina.
- **Kohalik režiim**: rühma liikmelisus ja võrgu liikmelisuse toimingud tuleks teostada [Microsoft 365 administraatori portaalist](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portaalist](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)või mõne muu Azure AD suvandi abil. Emakeelena režiimis olevatel võrkudel pole enam juurdepääsu lahtisele versioonile ja muudele varasematele funktsioonidele.

> [!IMPORTANT]
> Yammeri ei toetanud kunagi sisu importimist võrgu administraatorilt isegi siis, kui andmete eksportimise funktsiooni kasutati mõnes muus võrgus. Sisu saab uuesti postitada partnerite lahendused või Yammeri ülejäänud API-d.

**Eksportimine**

Võrgu [andmete eksportimine võrgu administraatori](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) kaudu lubab sisu eksportida Yammeri võrkudes (sh sõnumid ja failid). Manused võivad olla väga suured ja põhjustada eksportimisel olulise aja. Soovitame aktiivseid võrke eksportida, kasutades [andmete eksportimise API](https://developer.yammer.com/docs/data-export-api) -d iga päev või nädal. Microsoft support ei paku selleks kohandatud skripte.

Üksikute kasutajate jaoks sisu eksportimiseks on olemas eraldi [üldmääruse eksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) .