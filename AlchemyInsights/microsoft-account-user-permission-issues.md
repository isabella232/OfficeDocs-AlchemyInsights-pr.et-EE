---
title: Probleemi tõrkeotsing – kasutajat ei leitud kataloogist
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725403"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Probleemi tõrkeotsing – kasutajat ei leitud kataloogist

Kui kasutajad saavad tõrketeate "kasutaja ei leita", proovige uuesti, kui probleemi tüüp on kasutaja, kes pole kataloogis.

Probleemi tõrkeotsinguks saab teha järgmisi toiminguid.

- Veenduge, et e-posti kutse aktsepteeritud konto on sama konto, mida kasutatakse hiljem sisselogimiseks. Veenduge, et kasutaja kasutab sama kontot, et kutse vastu võtta ja saidile sisse logida. 

Lisateavet leiate teemast Microsofti [konto pseudonüümide haldamine </a> Microsoft 365 sisselogimise haldamiseks](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Sirvige iga saidi (te) ga, kus kasutaja tõrketeate saab. 

Lisage saidi URL-i lõppu "/_layouts/15/People.aspx/membershipgroupid = 0" (jutumärkides). 

Näide: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Valige loendist kasutaja.

- Klõpsake lindil nuppu **Eemalda kasutajaõiguste** . 
-  Lisage kasutaja tagasi ja saatke kutse uuesti kasutajale.

