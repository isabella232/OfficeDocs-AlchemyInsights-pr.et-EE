---
title: Levinud probleemide lahendamine DKIM-kirjevormingus
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323986"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Levinud probleemide lahendamine DKIM-kirjevormingus

Enamik DKIM-i häälestamisprobleeme on seotud valede DNS-i kirjetega.

DKIM-i häälestamisprobleemide lahendamiseks veenduge, et DKIM-i CNAME-kirje **(mitte** TXT-kirje) oleks õigesti vormindatud. Lisateavet leiate teemast Mida on vaja teha [DKIM-i](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)käsitsi häälestamiseks Office 365.

Kui vajate DNS-i kirjetega üldiselt abi, lugege teemat DNS-i kirjete loomine mis [tahes DNS-hostiteenuse pakkuja juures Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

**Märkus.** Pärast DKIM-i DNS-i kirjete lisamist või värskendamist oma domeeni DNS-hostiteenuses peate ootama, kuni DNS-i kirjed levivad.
