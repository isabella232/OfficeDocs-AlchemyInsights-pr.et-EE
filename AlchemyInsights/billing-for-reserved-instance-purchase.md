---
title: Arveldamine reserveeritud eksemplari ostmiseks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823074"
---
# <a name="billing-for-reserved-instance-purchase"></a>Arveldamine reserveeritud eksemplari ostmiseks

Reserveeritud eksemplari ost võetakse ostu sooritamise ajal valitud tellimusega seotud makseviisi. Tellimuse tüüp peab olema ettevõtte leping (pakkumise number: MS-AZR-0017P), tasuliste (pakkumise number: MS-AZR-0003P), Microsofti kliendi leping või CSP.

- Ettevõtte tellimuse puhul arvestatakse tasud maha liitumise rahalise kohustuse saldost või võetakse üle
- Tasulise tellimuse korral tasu võetakse tellimusel krediitkaardi või arve makseviisi arvel.

**Reserveeringu tühistamine**

- **Iseteeninduse teenus:** Reserveeritud eksemplari saate Azure ' i [portaali](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)kaudu ise tühistada või vahetada. Valige reserveerimine ja klõpsake nuppu tagasimakse või Exchange. Pidage meeles, et Exchange ' i või tagasimakse korral peab teil olema omaniku juurdepääs broneeringu korraldusele. Juurdepääs ainult broneeringule ei võimalda teil jätkata tagasimakset ega Exchange ' i. Paluge broneeringu korralduse omanikul anda teile omanikule juurdepääs broneeringu korraldusele.
- **Exchange ' i poliitika.** Saate vahetada reservatsiooni sama tüüpi broneeringu eest – broneeringute vahetuse korral pole **trahve** . Uue reservatsiooniga seotud kulukohustuste kogusumma peaks olema suurem kui Exchange ' i broneeringu tagasimakse summa ja tulevased igakuised maksed (vajaduse korral).
- **Tagasimakse põhimõtted:** Tagasimakse summa ja tühistatud tulevased maksed ei tohi 12-kuulise jooksvas aknas ületada $50 000 USD. Me ei nõua praegu tagasimaksete eest **karistusi** , vaid võivad selle eest tasuda ka tulevikus.

**Erandid.** Iseteenindusega Exchange ja loobumise võimalus pole USA valitsuse Enterprise ' i lepingu klientide jaoks saadaval

- **API/PS/CLI** tugi pole saadaval broneeringu tühistamiseks ja tagasimaksete jaoks, mida pakutakse [Azure ' i reserveerimiste jaoks](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Iseteenindusega Exchange ja loobumise võimalus pole USA valitsuse Enterprise ' i lepingu klientide jaoks saadaval. Toetatud on ka muud USA valitsuse tellimuse tüübid, sh tasulised ja riiklikud tellimused

Lisateavet leiate teemast tagasimaksed [ja Exchange ' i kanded töödeldakse](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) lähemalt: [Exchange ja tagasimakse poliitika](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) muud küsimused: [Külasta reserveeritud eksemplari docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Olemasoleva reserveeritud eksemplari vahetamine (iseteenindusega)**

Teise sama tüüpi broneeringu eest saate vahetada reservatsiooni. Soovi korral saate tagastada ka broneeringu, kuni $50 000 USD aastas, kui te seda enam ei vaja. Iseteenindusega Exchange ja loobumise võimalus pole USA valitsuse Enterprise ' i lepingu klientide jaoks saadaval. Toetatud on ka muud USA valitsuse tellimuse tüübid, sealhulgas tasuliste ja---uudiste liigid. Olemasoleva reservatsiooni vahetamiseks või tagasimaksmiseks peab teil olema omaniku juurdepääs broneeringu tellimusele.

Järgmised juhised juhivad tehingu sooritamise protseduuri.

1. logige sisse oma [Azure ' i portaali](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Valige reserveerimised, mida soovite tagastada, ja klõpsake nuppu **Exchange** 2. Valige VM toode, mida soovite osta, ja tippige kogus. Veenduge, et uus ostu kogusumma oleks suurem kui tagastamise kogusumma, mis [määrab enne ostu tegemist õige suuruse](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. tehingu läbivaatamine ja täiendamine

**Reserveeritud eksemplari tagasimakse**

Broneeringu tagasimaksmiseks Avage **broneeringu üksikasjad** ja klõpsake nuppu **tagastus** .

**Pro-reitinguga tagasimakse:**

**Tagasimaksete ja Exchange ' i Pro-ratione ja miinimumnõude näited** Ees broneeringu näide:

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

**Viimase arvelduse perioodi arvet ei kuvata.**

Mõned võimalikud põhjused, miks te arvet ei näe.

- Sul on oma tellimusega igakuine krediidi summa, mida sa ei ületanud või sul on tasuta prooviversioon. Arve luuakse ainult siis, kui võlgnete raha
- Azure ' i tellimusest on vähem kui 30 päeva.
- Arve pole veel loodud. Oodake kuni arvelduse perioodi lõpuni
- Kui te pole konto administraator, ei pruugi vanemad arved teie jaoks saadaval olla.

**Arve allalaadimine Azure ' i portaalist (. pdf)**

- Valige oma tellimus Azure ' i portaalis [tellimuste lehelt](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) [kasutajana, kellel on juurdepääs arvetele](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Vali **arved**
- PDF-i arve koopia vaatamiseks klõpsake nuppu **Laadi arve** . Kui see **pole saadaval** , lugege teemat [miks ei kuvata viimase arvelduse perioodi arvet?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Arve vastuvõtmine meili teel (. pdf)**

- Valige tellimus lehelt [tellimused](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Valige **Arveldamine ja seejärel** meili minu arve
- Klõpsake nuppu **Vali** ja Nõustuge tingimustega. Pead valima iga oma tellimuse eest.

Märkus: kui te ei saa pärast juhiseid juhiseid, siis veenduge, et teie meiliaadress oleks [teie profiilis suhtluse eelistustes](https://account.windowsazure.com/profile) õige.

**Andmete allalaadimine Azure ' i portaalist**

- Logige sisse [Azure ' i konto keskusse](https://account.windowsazure.com/Subscriptions) [konto administraatorina](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Valige tellimus, mille arve ja kasutusandmed soovite vaadata
- **Arvelduste ajaloo** valimine
- Kui soovite näha kalkulatsiooni loomise ajal oma tasude kalkulatsiooni, valige **Kuva praegune lause** .
- Igapäevase kasutuse andmete allalaadimiseks CSV-failina valige **Laadi alla kasutamine** . Kui kuvatakse kaks versiooni, Laadi alla versioon 2

Muud küsimused: [Külasta reserveeritud eksemplari docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Soovitatavad dokumendid**

- [Arvelduse põhitõed](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Saate teada, kuidas reserveeritud eksemplari hinnaalandit rakendatakse](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure ' i arvelduse arve ja igapäevase kasutuse andmete allalaadimine või vaatamine](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Saate teada, kuidas reserveeritud eksemplari hinnaalandit rakendatakse](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Saate teada, kuidas reserveeritud eksemplaride kasutus teie tasulise tellimuse korral](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Saate teada, kas teie ettevõtte registreerimine on reserveeritud eksemplaride kasutus](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windowsi tarkvara kulud, mida ei hõlma reserveeritud eksemplarid](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserveeritud eksemplarid partnerite keskses pilve lahenduste pakkuja (CSP) programmis](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)