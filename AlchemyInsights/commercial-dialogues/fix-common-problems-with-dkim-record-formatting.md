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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930057"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Levinud probleemide lahendamine DKIM-kirjevormingus

Enamik DKIM-i häälestamisprobleeme on seotud valede DNS-i kirjetega.

DKIM-i häälestamisprobleemide lahendamiseks veenduge, et DKIM-i CNAME-kirje **(mitte** TXT-kirje) oleks õigesti vormindatud. Lisateavet leiate teemast Mida on vaja teha [DKIM-i](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)käsitsi häälestamiseks Office 365.

Kui vajate dns-i kirjetega üldiselt abi, lugege teemat DNS-i kirjete loomine mis [tahes DNS-hostiteenuse pakkuja juures Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Pärast DKIM-i DNS-i kirjete lisamist või värskendamist oma domeeni DNS-hostiteenuses peate ootama, kuni DNS-i kirjed levivad.
