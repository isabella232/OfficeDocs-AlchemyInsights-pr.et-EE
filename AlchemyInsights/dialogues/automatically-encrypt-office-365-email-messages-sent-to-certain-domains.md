---
title: Office 365 meilisõnumite automaatne krüptimine teatud domeenidele saadetavate meilisõnumite jaoks
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524872"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Office 365 meilisõnumite automaatne krüptimine teatud domeenidele saadetavate meilisõnumite jaoks

1. Valige [Exchange ' i administreerimiskeskuses](https://outlook.office365.com/ecp/)suvand **mail Flow > reeglid**. 
2. Klõpsake ikooni **Uus (+)** ja seejärel käsku **Rakenda Office 365 Sõnumite krüptimine ja õiguste kaitse sõnumitele**.
3. Sisestage väljale **nimi** reegli nimi (nt *contoso.com saadetud sõnumite krüptimine*).
4. **Kui olete selle reegli rakendanud**, valige **adressaadi > Domeen**. 
5. Sisestage domeeni nimi (nt **contoso.com**).
6. Klõpsake ikooni **Add (+) (+)** ja seejärel klõpsake nuppu **OK**.
7. Klõpsake välja " **tee järgmine** " kõrval nuppu **Vali see**. 
8. Valige rippmenüüs **RMS** -i Mall käsk **Krüpti** ja seejärel klõpsake nuppu **OK**. (Kui seda suvandit ei kuvata, tähendab see seda, et teie leping ei sisalda automaatset krüptimist. Kuid saate selle lisada!)
9. Valige mis tahes valikuline valik (loendist valikuliste valikute seast, mida saate selles punktis teha, millest paljusid saab lisada lihtsuse vaikesätetega).
10. Klõpsake nuppu **Salvesta**.

> [!IMPORTANT]
> Saate alati tagasi tulla ja seda reeglit hiljem redigeerida.

Lisateavet krüptimise reeglite loomise kohta leiate teemast meilisõnumite [krüptimine meilisõnumite krüptimiseks Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)