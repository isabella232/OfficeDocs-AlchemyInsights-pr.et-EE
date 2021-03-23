---
title: Azure AD Authenticationi ja autoriseerimise (AADSTS) tõrkekoodid tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035637"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Azure AD Authenticationi ja autoriseerimise (AADSTS) tõrkekoodid tõrkeotsing

AAD autentimise ja autoriseerimise tõrkekoodid (AADSTS) lahendamiseks tehke järgmised Soovitatavad toimingud.

1. **Rakenduse tõrkekoodid käitlemine**

- **OAuthi 2.0 spec**, annab juhiseid selle kohta, kuidas tõrke korral tõrkeid tõrkeid https://tools.ietf.org/html/rfc6749#section-5.2 kasutades autentida.

    - **tõrge**: tõrkekood string, mida saab kasutada ilmnevate tõrgete tüüpide klassifitseerimiseks, ning seda tuleks kasutada tõrgete korral reageerimiseks.
    - Väljal **viga** on mitu võimalikku väärtust – vaadake üle protokolli dokumentatsiooni lingid ja OAuthi 2,0 specs, et saada lisateavet konkreetsete tõrgete ja neile reageerimise kohta.

- Siin on proovi tõrge vastus:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Praeguse tõrke koodi teabe otsing**

- Tõrkekoodid ja sõnumid võivad muutuda. Uusimat teavet leiate https://login.microsoftonline.com/error lehelt AADSTS vigade kirjeldused, parandused ja Soovitatavad lahendused.
- Samuti saate otsida ja sooritada artiklis [AZURE ad autentimine ja autoriseerimise](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)tõrkekoodid loetletud [AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) .

3. **Abi saamine**

- [Arendajate tugi-ja tugikeskused](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – kui vajate vastust küsimusele või abi, mis lahendab probleemi, mida meie dokumentatsioon ei hõlma, võib olla aeg saada abi ekspertidele. Selles artiklis on esitatud mitu soovitust, kuidas saada oma küsimustele vastuseid, kui arendate rakendusi, mis integreeritakse Microsoft Identity platformiga.








