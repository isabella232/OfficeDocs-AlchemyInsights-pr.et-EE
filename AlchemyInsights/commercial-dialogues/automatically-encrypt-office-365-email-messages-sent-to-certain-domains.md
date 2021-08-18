---
title: Teatud Office 365 saadetud meilisõnumite automaatne krüptimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318844"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Teatud Office 365 saadetud meilisõnumite automaatne krüptimine

1. Valige [Exchange halduskeskuses](https://outlook.office365.com/ecp/) **meilivoog ja > reeglid**. 
2. Klõpsake ikooni **Uus (+)** ja seejärel käsku Rakenda **Office 365 sõnumikrüptimine ja õiguste kaitse sõnumitele.**
3. Sisestage väljale Nimi reegli nimi (nt Krüpti sõnumeid, *mis on saadetud contoso.com*). 
4. Valige **jaotises Rakenda see reegel, kui**> **on** adressaat. 
5. Sisestage domeeni nimi (nt **contoso.com).**
6. Klõpsake ikooni **Lisa (+)** ja seejärel nuppu **OK**.
7. Klõpsake välja **Do the following (Tehke järgmist)** kõrval nuppu Select one **(Vali üks).** 
8. Valige **RMS-malli** rippmenüüs **Krüpti ja** seejärel klõpsake nuppu **OK**. (Kui seda suvandit ei näe, tähendab see, et teie leping ei sisalda automaatset krüptimist. Kuid saate selle lisada!)
9. Valige mis tahes valikuline valik (valikuliste valikute loendist, mida saate praegu teha, millest paljud võivad olla jäänud lihtsuse vaikesätteks).
10. Klõpsake nuppu **Salvesta**.

**Tähtis.** Saate alati tagasi tulla ja seda reeglit hiljem redigeerida.

Lisateavet krüptimisreeglite loomise kohta leiate teemast [Meilivooreeglite määratlemine meilisõnumite](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) krüptimiseks Office 365