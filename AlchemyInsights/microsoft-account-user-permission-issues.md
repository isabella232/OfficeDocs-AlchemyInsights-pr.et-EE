---
title: Tõrkeotsing – kasutajat ei leitud kataloogist
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098166"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Tõrkeotsing – kasutajat ei leitud kataloogist

Kui kasutajad saavad kataloogist tõrketeadet "kasutajat ei leita", proovige uuesti, kui probleemi tüüp pole kasutaja kataloogis.

Probleemi tõrkeotsinguks saate teha järgmised toimingud.

- Veenduge, et meilikutse aktsepteerinud konto oleks sama konto, mida kasutatakse hiljem sisselogimiseks. Veenduge, et kasutaja kasutaks kutse aktsepteerimiseks ja saidile sisselogimiseks sama kontot. 

Lisateavet leiate teemast Microsofti konto pseudonüümide haldamine sisselogimise [ </a> Microsoft 365.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Liikuge sirvides iga saidi(te)ni, kus kasutaja vea saab. 

Lisage saidi URL-i lõppu "/_layouts/15/people.aspx/membershipgroupid=0" (jutumärkides). 

Näide: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Valige loendist kasutaja.

- Klõpsake **lindil nuppu Eemalda** kasutajaõigused. 
-  Lisage kasutaja tagasi ja saatke kutse kasutajale uuesti.

