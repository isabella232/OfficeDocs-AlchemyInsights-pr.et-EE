---
title: S/MIME Outlooki veebirakendus
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010720"
---
# <a name="encrypt-email-messages-in-outlook"></a>Meilisõnumite krüptimine Outlook

Microsoft 365 Sõnumikrüptimine põhineb Azure'i teabekaitse osaks oleval Microsoft Azure Rights Managementi (Azure RMS) versioonil. Kui teie tellimus sisaldab Azure Rights Managementi või Azure'i teabekaitset, ei pea te õiguste halduse teenuse **käsitsi** lubamiseks ega aktiveerimiseks midagi tegema.

Klientide tagasiside põhjal ei luba me enam meilivoo Exchange reeglitel automaatselt krüptida väljaminevaid meilisõnumeid, mis sisaldavad teie rentnikus teatud tüüpi tundlikku teavet. Selle asemel anname teile üksikasjalikud juhised selle kohta, kuidas saate seda ise teha. Lisateavet tundliku teabe krüptimiseks transpordireegli loomise kohta leiate sellest [artiklist.](https://aka.ms/OmeEtr)

- Kui kasutate Outlook (varem **OWA):** Meilisõnumi koostamisel klõpsake lihtsalt käsku **Kaitse** OWA-s. See kehtib "Ära saada edasi". Klõpsake **nuppu Muuda õigusi** ja valige **Krüpti** ainult sõnumi krüptimiseks.

- Kui **kasutate Outlook** klientrakendust: krüptitud sõnumi saatmiseks opsüsteemist Outlook 2013 või 2016 või Outlook 2016 for Mac valige **Suvandid** õigused ja seejärel valige soovitud  >  kaitsesuvand.

- Teatud **adressaatidele või välistele** partnerorganisatsioonidele saadetud meilisõnumite automaatseks krüptimiseks peate looma meilivoo transpordireegli Exchange halduskeskuses. Üksikasjalikud juhised leiate sellest [tugiteenuste artiklist.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

