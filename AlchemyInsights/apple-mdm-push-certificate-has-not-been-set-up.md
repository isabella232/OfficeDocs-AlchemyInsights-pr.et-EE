---
title: Apple MDM push ' i serti pole häälestatud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439013"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM push ' i serti pole häälestatud

Apple MDM push Certificate (tuntud ka kui Apple push Notification Service (APNS) sert) pole teie tellimuse jaoks konfigureeritud. Kui Apple MDM push Certificate pole konfigureeritud, ei saa te iOS-i ja Mac OS-i seadmeid registreerida ja hallata. Kui olete serdi lisamiseks Intune ' i lisanud, saavad kasutajad oma iOS-i seadmete registreerimiseks installida ettevõtte portaali rakenduse.

1. Valige **"Nõustun".** anda Microsoftile luba andmete saatmiseks Apple ' i.

2. Valige **Laadi alla oma CSR** -i Intune ' i serdi allkirjastamise taotlus, mis on vajalik Apple MDM push-serdi loomiseks. Seda faili kasutatakse Apple ' i push Certificates portaalis usalduse suhte serdi taotlemiseks.

3. Klõpsake nuppu **Loo MDM-push** ' i sert, et minna Apple Pushi sertide portaali. Logige sisse oma ettevõtte Apple ID-ga ja seejärel valige **Loo sert**. Valige Vali **pilt**, sirvige serdi allkirjastamise taotluse failini ja seejärel klõpsake käsku **Laadi üles**. Serdi (. PEM) faili allalaadimiseks klõpsake lehel kinnitus nuppu **Laadi alla** ja salvestage faili kohalikult.
 
**Märkus**: sert on seotud selle loomiseks kasutatava Apple ID-ga. Parima tavana Kasuta ettevõtte Apple ID-ga haldustoiminguid ja veenduge, et postkasti jälgitakse rohkem kui ühe isiku või leviloendi abil. Ära kasuta isikliku Apple ' i ID-ga. Apple Pushi serdi uuendamiseks iga 12 kuu järel kasutage sama Apple ' i ID-ga.
 
4. Apple MDM push ' i serdi loomiseks kasutatava Apple ' i ID sisestamine. Registreerige see ID meeldetuletuseks, kui teil on vaja serti uuendada.

5. Avage faili sert (. PEM), valige **Ava**ja seejärel klõpsake nuppu **Laadi üles**. Push Certificate abil saab Intune ' i registreeruda ja hallata Apple ' i seadmeid.