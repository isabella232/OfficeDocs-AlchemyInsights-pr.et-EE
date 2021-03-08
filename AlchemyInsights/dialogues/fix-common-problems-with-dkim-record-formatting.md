---
title: Levinud probleemide lahendamine DKIM kirje vorminguga
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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524399"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Levinud probleemide lahendamine DKIM kirje vorminguga

Enamik DKIM on seotud valede DNS-i kirjetega.

DKIM lahendamiseks veenduge, et DKIM CNAME-kirje (**mitte** TXT-kirje) oleks õigesti vormindatud. Lisateavet leiate teemast [mida peate tegema DKIM käsitsi häälestamiseks rakenduses Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Kui vajate DNS-i kirjete üldist abi, lugege teemat [DNS-i kirjete loomine veebisaidil Office 365 DNS-i majutusteenuse pakkuja](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Pärast seda, kui olete oma domeeni DNS-i DKIM loonud või värskendanud DNS-i kirjeid, peate ootama, kuni DNS-i kirjed on paljundatud.
