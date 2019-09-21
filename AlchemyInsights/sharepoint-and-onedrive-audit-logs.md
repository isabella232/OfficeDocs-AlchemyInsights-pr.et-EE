---
title: Klassikaline SharePointi auditilogi aruanded
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068019"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePointi ja OneDrive ' i auditilogi

**SharePointi ja OneDrive kaasaegne ühendatud audit logib vastavuse**

- [Lülita sisse/välja ühendatud auditilogi logimine](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

SharePoint või OneDrive ei vaja täiendavat konfiguratsiooni.

- Auditilogi otsingu abil saate kontrollida faili (de), kausta (de), kasutaja (te), õigusi:

    - [Faili-ja lehetegevused](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Kausta tegevused](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Jagamise ja juurdepääsu taotluse tegevused](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Sünkroonimise tegevused](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Saidihalduse tegevused](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Lisateavet nende sündmuste kohta leiate teemast [auditilogi otsing](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**SharePointi klassikaline auditilogi**

Me migreerisime SPO pärand auditeerimine Unified audit log (UAL). See tähendab sisuliselt, et kõik SPO pärand auditiaruanded on nüüd läbi UAL ja pärand auditi signaale on migreeritud UAL.

Peamised muudatused:

- Korrastamine võimetena ei ole saadaval.
- Jaotis, kus saate auditeerimiseks konkreetseid sündmusi valida, pole saadaval. Palun vaadake [seda dokumenti](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) vaikimisi saadaolevate auditeeritud sündmuste täieliku loendi kohta.
- **Kohandatud aruannete** all suvand "asukoht" pole saadaval. 
- "Dokumentide avamine või allalaadimine" sündmused pole saadaval. 

