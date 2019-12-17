---
title: Probleemi tõrkeotsing-kasutajat ei leitud kataloogist
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054806"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Probleemi tõrkeotsing-kasutajat ei leitud kataloogist

Kui kasutajad saavad tõrketeate "kasutajat ei leita" kataloogis, proovige uuesti, kui probleemi tüüp on kasutaja ei ole kataloog.

Järgmised sammud saab lõpule viia probleemi tõrkeotsingu sooritamiseks.

- Veenduge, et e-posti kutse aktsepteeritud konto on sama konto, mida kasutatakse hiljem sisse logida. Veenduge, et kasutaja kasutab sama kontot kutse vastuvõtmiseks ja saidile sisselogimiseks. 

Lisateabe saamiseks vaadake, [Kuidas hallata pseudonüümid oma Microsofti konto</a> hallata Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Sirvige iga saidi (s), kus kasutaja saab tõrke. 

Lisage "/_layouts/15/People.aspx/membershipgroupid = 0" (sees kahekordsete jutumärkidega) saidi URL-i lõppu. 

Näide: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Valige loendist kasutaja.

- Klõpsake lindilt **kasutaja õiguste eemaldamine** . 
-  Lisa kasutaja tagasi ja saatke kutse kasutajale.

