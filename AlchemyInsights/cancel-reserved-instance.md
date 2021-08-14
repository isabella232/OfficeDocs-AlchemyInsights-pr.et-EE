---
title: Reserveeringu tühistamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931229"
---
# <a name="cancelling-reservation"></a>Reserveeringu tühistamine

- **Iseteenindus:** Reserveeritud eksemplari saate azure'i portaali kaudu ise tühistada [või vahetada.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Valige broneering ja klõpsake tagasimakset või vahetust. Võtke arvesse, et teil peab olema omaniku juurdepääs broneerimiskorraldusele, et seda vahetada või tagasi maksta. Juurdepääs ainult broneeringule ei luba teil tagasimakset või vahetust jätkata. Paluge reserveerimistellimuse omanikul anda teile omanikule juurdepääs reserveerimiskorraldusele.
- **Exchange poliitika:** Saate vahetada reserveeringut mõne muu sama tüüpi reserveeringu vastu – broneeringu vahetamisel **ei ole** mingeid karistusi. Uue reserveeringuga kogukohustus peaks olema suurem kui vahetatud broneeringu tagasimakse summa ja tulevased igakuised maksed (kui see on asjakohane)
- **Tagasimaksepoliitika:** Tagasimaksesumma ja tühistatud tulevased maksed ei tohi ületada 50 000 USA dollarit 12-st kuust jooksvas aknas. Me ei **pea praegu tagasimaksete eest mingit** karistust, kuid võime selle tulevaste tagasimaksete eest tasuda.  
    **Erandid:** Iseteeninduslik vahetus ja tühistamisvõimalus pole SAADAVAL USA Enterprise Agreement klientidele
- **API / PS / CLI** tugi ei ole saadaval tühistamiseks ja tagasimaksete makstes Azure'i broneeringute iseteeninduse [vahetused ja tagasimaksed](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Iseteeninduslik vahetus ja tühistamisvõimalus pole SAADAVAL USA Enterprise Agreement klientidele. Toetatakse muid USA valitsuse tellimuse tüüpe, sh Pay-As-You-Go ja CSP

Lisateave: [Tagastus- ja vahetustehingute töötlemine](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Lisateave: [Exchange tagasimaksepoliitikad](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Muud küsimused: [külastage reserveeritud eksemplariga dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange reserveeritud eksemplari (iseteenindus)**

Saate vahetada reserveeringut mõne muu sama tüüpi reserveeringu vastu. Kui te seda enam ei vaja, saate broneeringu tagasi maksta kuni 50 000 USA dollarit aastas. Iseteeninduslik vahetus ja tühistamisvõimalus pole SAADAVAL USA Enterprise Agreement klientidele. Toetatakse muid USA valitsuse tellimuse tüüpe, sh Pay-As-You-Go ja CSP. Olemasoleva broneeringu vahetamiseks või tagastamiseks peab teil olema omaniku juurdepääs broneerimiskorraldusele.

Tehingu lõpuleviimiseks tehke järgmist.

1. Logige sisse Oma [Azure'i portaali.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Valige broneeringud, mille soovite tagasi maksta, ja klõpsake **nuppu Exchange**
2. Valige VM-toode, mida soovite osta, ja tippige kogus. Veenduge, et uue ostu kogusumma oleks suurem kui tagastussumma. Määrake [enne ostmist õige suurus](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Tehingu läbivaatamine ja lõpule viimine

**Reserveeritud eksemplari tagasimakse**

Broneeringu tagastamiseks minge valikusse Broneeringu üksikasjad **ja** klõpsake nuppu **Tagasimakse.**

**Pro tagasimakse:**

**Pro ja miinimumnõude näited raha tagastamise ja vahetamise kohta**  
Ettetellimise näide:

- Ostate 1. jaanuaril 120-ga üheaastase tähtajaga RI
- 7. aprillil soovite selle broneeringu tagasi maksta või vahetada
- Kuna broneering on 97 päeva jooksul reaalajas olnud, saate (1-97/365) * 120 $ tagasi. (st 88,1 $ ). Tagasimaksete eest praegu karistust ei määrata
- Vahetamise korral peaks teie uus ost olema suurem kui 88,1 $
- Praegu tagasimaksete eest karistust ei määrata

**Arveldusplaani reserveerimise näide:**

- Ostate üheaastase tähtajaga RIT-d 10 $ kuus
- 7. aprillil soovite selle broneeringu tagasi maksta või vahetada
- Kuna viimane makse on tehtud 7 päeva, saate (1-7/31) * 10 $ tagasi. (st 7,74 $)
- Tühistatud tulevased maksed on 80 $. Tagasimaksete eest praegu karistust ei määrata
- Tühistamine lahutab teie 50 000 $ tagasimakselimiidist 87,74 $
- Vahetamise korral peaks uue ostu koguväärtus olema suurem kui 87,74 $

**Soovitatud dokumendid**

- [Tagastus- ja vahetustehingute töötlemine](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange ja tagasimakse poliitikad](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)