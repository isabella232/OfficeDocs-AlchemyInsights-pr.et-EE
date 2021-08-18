---
title: Domeeni olek – teenuseid pole valitud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 2247da07d60431edef5b5dea8a5c06d51579008c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326573"
---
# <a name="domain-status---no-services-selected"></a>Domeeni olek – teenuseid pole valitud

**Ükski teenus pole valitud** tähendab, et te pole Microsoft 365 (nt Exchange Online, Skype'i ärirakendus või Intune) ega mobiilsideseadmete haldust Microsoft 365 kohandatud domeeniga kasutamiseks. Kui kasutate Exchange hübriidfiltrit (Exchange on kohapealne Exchange Online) või välise rämpsposti filtreerimist Exchange ja muid Microsofti teenused, saate seda teadet eirata. Domeeni seisundi olek on saadaval ainult domeenide jaoks, mis on otse teenusega ühendatud.

Oma domeeni jaoks teenuste valimiseks tehke seda.

1. Märkige **Sätted**  >  [**domains**](https://admin.microsoft.com/Adminportal/Home)(Domeenid) selle domeeni kõrval ruut, kus olekuteade **Pole teenuseid valitud**.
1. Domeeni **häälestusviisardi** käivitamiseks valige Halda DNS-i.
    - Kui valite **käsu Lisa oma DNS-i** kirjed, valige küsimisel kindlasti teenus. Rohkem teenuseid võib olla saadaval jaotises **Täpsemad suvandid.**
    - Kui valite **Suvandi Luba Microsoftil lisada oma DNS-i** kirjeid või **Rohkem** suvandeid Häälesta minu jaoks minu jaoks kõik  >   saadaolevad teenused soovitatakse ja valitakse automaatselt.
1. Dns-i häälestamise ja teenusevalikute lõpuleviimiseks jätkake viisardi kaudu.
 
Lisateavet domeeni häälestamise kohta leiate teemast [DNS-i kirjete lisamine domeeni ühendamiseks.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

