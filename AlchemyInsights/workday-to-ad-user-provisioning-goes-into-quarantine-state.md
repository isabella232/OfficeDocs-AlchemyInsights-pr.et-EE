---
title: Workday to AD User Provisioning läheb karantiini olekusse
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036488"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday to AD User Provisioning läheb karantiini olekusse

**Tööpäev AD kasutajaks ettevalmistamine läheb karantiini olekusse ja AD-s ei looda kasutajaid**

Tööpäev AD kasutajaks ettevalmistamise töö on karantiini olekusse läinud ja auditilogides kuvatakse eksporditõrked tõrketeatega **Tõrge: OperationsError-SvcErr: ilmnes toimingutõrge. Kataloogiteenuse jaoks pole ühtegi kõrgemat viidet konfigureeritud. Kataloogiteenus ei saa seetõttu väljastada viiteid väljaspool seda metsa asuvate objektide kohta.** See tõrge kuvatakse tavaliselt siis, kui Active Directory ümbrise OU pole õigesti määratud või kui on probleeme **parentDistinguishedNamei jaoks kasutatava avaldisevastendusega.**

Kontrollige parameetrit Vaike-OU uute kasutajate **jaoks,** et leida kirjavead. Veenduge, et määratud OU on teie AD-s juba olemas. Kui kasutate **atribuudivastenduses parentDistinguishedNamei,** veenduge, et selle väärtus oleks AD-domeenis alati teadaolev ümbris. Kontrollige genereeritud väärtuse näeks auditilogides sündmust Ekspordi.

Lisateavet automaatseks ettevalmistamiseks tööpäevade konfigureerimise kohta leiate teemast [Õpetus: Tööpäeva konfigureerimine automaatseks kasutajate ettevalmistamiseks.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

