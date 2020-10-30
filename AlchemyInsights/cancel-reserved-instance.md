---
title: Reserveeringu tühistamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807568"
---
# <a name="cancelling-reservation"></a>Reserveeringu tühistamine

- **Iseteeninduse teenus:** Reserveeritud eksemplari saate Azure ' i [portaali](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)kaudu ise tühistada või vahetada. Valige reserveerimine ja klõpsake nuppu tagasimakse või Exchange. Pidage meeles, et Exchange ' i või tagasimakse korral peab teil olema omaniku juurdepääs broneeringu korraldusele. Juurdepääs ainult broneeringule ei võimalda teil jätkata tagasimakset ega Exchange ' i. Paluge broneeringu korralduse omanikul anda teile omanikule juurdepääs broneeringu korraldusele.
- **Exchange ' i poliitika.** Saate vahetada reservatsiooni sama tüüpi broneeringu eest – broneeringute vahetuse korral pole **trahve** . Uue reservatsiooniga seotud kulukohustuste kogusumma peaks olema suurem kui Exchange ' i broneeringu tagasimakse summa ja tulevased igakuised maksed (vajaduse korral).
- **Tagasimakse põhimõtted:** Tagasimakse summa ja tühistatud tulevased maksed ei tohi 12-kuulise jooksvas aknas ületada $50 000 USD. Me ei nõua praegu tagasimaksete eest **karistusi** , vaid võivad selle eest tasuda ka tulevikus.  
    **Erandid.** Iseteenindusega Exchange ja loobumise võimalus pole USA valitsuse Enterprise ' i lepingu klientide jaoks saadaval
- **API/PS/CLI** tugi pole saadaval broneeringu tühistamiseks ja tagasimaksete jaoks, mida pakutakse [Azure ' i reserveerimiste jaoks](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Iseteenindusega Exchange ja loobumise võimalus pole USA valitsuse Enterprise ' i lepingu klientide jaoks saadaval. Toetatud on ka muud USA valitsuse tellimuse tüübid, sh tasulised ja riiklikud tellimused

Lisateave: [tagasipöördumine ja Exchange ' i tehingute töötlemine](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Lisateave: [Exchange ' i ja tagasimakse põhimõtted](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Muud küsimused: [Külasta reserveeritud eksemplari docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Olemasoleva reserveeritud eksemplari vahetamine (iseteenindusega)**

Teise sama tüüpi broneeringu eest saate vahetada reservatsiooni. Soovi korral saate tagastada ka broneeringu, kuni $50 000 USD aastas, kui te seda enam ei vaja. Iseteenindusega Exchange ja loobumise võimalus pole USA valitsuse Enterprise ' i lepingu klientide jaoks saadaval. Toetatud on ka muud USA valitsuse tellimuse tüübid, sealhulgas tasuliste ja---uudiste liigid. Olemasoleva reservatsiooni vahetamiseks või tagasimaksmiseks peab teil olema omaniku juurdepääs broneeringu tellimusele.

Järgmised juhised juhivad tehingu sooritamise protseduuri.

1. Logige sisse oma [Azure ' i portaali](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Valige reserveerimised, mida soovite tagastada, ja klõpsake nuppu **Exchange**
2. Valige VM toode, mida soovite osta, ja tippige kogus. Veenduge, et uus ostu kogusumma oleks suurem kui tagastamise kogusumma, [enne kui ostate õige suuruse.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Tehingu läbivaatamine ja täiendamine

**Reserveeritud eksemplari tagasimakse**

Broneeringu tagasimaksmiseks Avage **broneeringu üksikasjad** ja klõpsake nuppu **tagastus** .

**Pro-reitinguga tagasimakse:**

**Tagasimaksete ja Exchange ' i Pro-ratione ja miinimumnõude näited**  
Ees broneeringu näide:

- Ostad üheaastase tähtaja RI for $120 jaanuaril 1
- 7. aprillil soovite selle reservatsiooni tagasi maksta või seda vahetada
- Kuna broneering on 97 päeva jooksul ellu viidud, saad (1-97/365) * $120 tagasi. (st $88,1). Tagasimaksete eest ei ole praegu karistust
- Vahetamise korral peaks uus ost olema suurem kui $88,1.
- Praegu ei ole trahve antud

**Arvelduse plaani Reservation näide:**

- Ostad üheaastase tähtaja RI for $10 kuus
- 7. aprillil soovite selle reservatsiooni tagasi maksta või seda vahetada
- Kuna Viimane makse juhtus 7 päeva pärast, saad (1-7/31) * $10 tagasi. (st $7,74)
- Tulevased maksed tühistati on $80. Tagasimaksete eest ei ole praegu karistust
- See tühistamine arvestab maha $87,74 alates sinust on $50 000 tagasimakse limiit
- Vahetamise korral peaks uue ostu koguväärtus olema suurem kui $87,74.

**Soovitatavad dokumendid**

- [Tagasisaatmis-ja Exchange ' i tehingute töötlemine](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange ' i ja tagasimakse põhimõtted](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)