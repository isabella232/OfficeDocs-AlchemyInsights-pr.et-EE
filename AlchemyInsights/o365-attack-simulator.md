---
title: 2681 rünnak simulaator Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713462"
---
# <a name="attack-simulator-in-microsoft-365"></a>Rünnak simulaator Microsoft 365

- Kas teil puudub rünnak simulaator? Rünnak simulaator nõuab **office 365 täiustatud ohutõrje kava 2 (ATP plaan 2)** või **Office 365 Enterprise E5**. Rünnak simulaator **ei** sisaldu Office 365 täiustatud ohutõrje kava 1 (ATP leping 1), Office 365 Enterprise E3 või mis tahes Microsoft 365 apps Business tellimused.

- Modelleeritud rünnakute käivitamiseks kasutatav konto nõuab globaalset administraatori või turbeülema õigusi ja mitme teguriga autentimist (MFA). Rünnaku simulaatori nõuete kohta lisateabe saamiseks vaadake [seda teemat](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Olulised asjad teada **Brute Force parooli** rünnaku simulatsioone:

  - Kui sihtkontol on MFA lubatud ja parool on õigesti arvatud, ei kuvata kontot ohustena (teine autentimistegur on puudulik).

  - Paroolifail ei tohi olla suurem kui 10 MB. Kasutage üks parool rea kohta ja lisage tühi rida (veo tagastamine) pärast viimast parooli loendis.

- Olulised asjad, mida teada **Spear phishing** lisada simulatsioone:

  - Ette nähtud, ei saa anda kohandatud väärtus **phishing logimisserveri URL-i**.

  - Kui adressaat kasutab sõnumi andmepüügi lubamiseks aruande sõnumi [lisandmoodul](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , te ei pruugi saada teatisi sõnumi (kuna see on simuleeritud rünnak).

- Aruanded: pärast simuleeritud rünnak on lõpule jõudnud, võite klõpsata **rünnak üksikasjad** aruande vaatamiseks.

- Üksikasjalikke juhiseid ja uusi funktsioone Attack Simulator, vt [rünnak simulaator Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
