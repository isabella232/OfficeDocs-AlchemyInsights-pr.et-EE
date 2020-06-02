---
title: 'AIP: poliitikad ei käitudes ootuspäraselt'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493022"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: poliitikad ei käitudes ootuspäraselt

Azure ' i teabekaitse: poliitikad ei käitudes ootuspäraselt, vt soovitatud juhised erinevate poliitikafunte:

1. Kui teil on visuaalsete märgistuste probleemid, vaadake üle [visuaalsete märgiste kohaldamise](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)korral.
2. Kui teil on probleeme automaatse märgistamise, vaadake üle, [Kuidas konfigureerida tingimused automaatse ja soovitatud klassifitseerimise Azure ' i teabekaitse](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mida tundliku teabe tüübid otsida](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
3. Kui teil on probleeme Native/Pfile kaitse, vaadake [faili API konfiguratsiooni](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontrollige, kas kasutate hõlmavaid poliitikaid, mis pole õigesti konfigureeritud: [Kuidas konfigureerida Azure ' i teabe kaitse poliitika teatud kasutajatele, kasutades ulatatud poliitikad](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Kui automaatne märgistamine ei tööta Outlooki sildistatud dokumendi ühendamisel, veenduge, et DRMEncryptProperty pole määratletud siin kirjeldatud: [IRM registrisätted turvalisuse](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Kui teil on endiselt probleeme, palun koguda Azure ' i teabe kaitse kliendi logid ja kinnitage eksporditud logid sellele piletile.

1. Avage Office ' i dokument või looge Outlookis uus e-kiri.
2. Klõpsake valikul **kaitse/tundlikkuse**  >  **Spikker ja tagasiside**.
3. Klikkige käsul **ekspordi logid**.
4. Salvestage logid oma asukoha valikule ja kinnitage need selle teenusetaotlusega.

Lisaressursid:

- [Kuidas konfigureerida sildile visuaalseid märgistusi Azure ' i teabekaitse](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure ' i teabekaitse dokumentatsiooni läbivaatamine](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Tundlikkuse siltide kasutamine Office ' i rakendustes](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

